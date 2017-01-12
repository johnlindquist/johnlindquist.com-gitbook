```
import {map, split, objOf} from 'ramda'

const alphabet = "abcdefghijklmnopqrstuvwxyz"

//converts the alphabet to [{letter: "a"}, {letter: "b"}, {letter: "c"}]
const lettersArray = map(objOf('letter'))(split('')(alphabet))

const LetterButton = props => <button key={props.letter}>{props.letter}</button>

//map over the letters array, pass each letter object as the props of the LetterButton
export default () => <div>{map(LetterButton)(lettersArray)}</div>
```