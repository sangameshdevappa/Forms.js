import axios from 'axios'
import { useState } from 'react'

function Forms() {

  //post request along with form data
  const [username, setUsername] = useState('')
  const [email, setEmail] = useState('')
  const [password, setPassword] = useState('')

  const handleFormSubmit = async() => {
    const resp = await axios.post("http://localhost:8080/formData", 
                                {username, email, password});
    console.log(resp)
  }
  return (
    <div>
      <form onSubmit={handleFormSubmit}>
          <label>Username : </label>
          <input type='text'
                 name='username'
                 value={username}
                 onChange = { (e) => setUsername(e.target.value) }
          />
          <br></br><br></br>
          <label>Email : </label>
          <input type='text'
                 name='email'
                 value={email}
                 onChange = { (e) => setEmail(e.target.value) }
          />
          <br></br><br></br>
          <label>Password : </label>
          <input type='text'
                 name='password'
                 value={password}
                 onChange = { (e) => setPassword(e.target.value) }
          />
          <br></br><br></br>
          <input type='submit' value='SUBMIT FORM' />
      </form>

    </div>
  );
}

export default Forms;
