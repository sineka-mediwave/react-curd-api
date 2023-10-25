# React CRUD Operation

- create your react app
- install these packages
  `npm install react-router-dom axios bootstrap json-server`
- Create pages to route (Create, Home, Read, Update)
- route the pages with app
- fetch data form the server

```
  const [data, setData] = useState<IUser[]>([]);
  useEffect(() => {
    axios
      .get("http://localhost:3000/users")
      .then((res) => setData(res.data))
      .catch((err) => console.log(err));
  }, []);
```
