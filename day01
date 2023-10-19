const express = require('express')
var cors = require('cors')
const app = express()
const port = 3000

app.use(cors())

app.get('/', (req, res) => {
  res.send('Hello World!~~~~')
})
app.get('/user/:id', (req, res) => {
    // const q = req.params
    // console.log(q.id)
    const q = req.query
    console.log(q.name)

    res.json({'name': q.name})
})  
app.get('/sound/:name', (req, res) => {
    const { name } = req.params // {} 사용시 value값이 name에 입력됨

    if( name == "cat" ) {
        res.json({'sound':'야옹'})
    } else if( name == "dog" ) {
        res.json({'sound':'멍멍'})
    } else {
        res.json({'sound':'알수없음'})
    }
})  

app.listen(port, () => {
  console.log(`Example app listening on port ${port}`)
})
