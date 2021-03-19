#Como se usa:

En mi funciones:
```
        const initialForm = {
        textoInput: '',
    }
    const [formValues, handleInputChange,reset] = useForm(initialForm);
    const {textoInput} = formValues;
    
        const handleSearch = (e) =>{
        e.preventDefault();
        console.log(formValues);
    }

```
En mi html:
```
                    <form onSubmit={handleSearch}>
                        <input
                            type="text"
                            placeholder="Tu texto"
                            name="textoInput"
                            value={textoInput}
                            onChange={handleInputChange}
                        />
                        <button
                            type="submit"
                            onClick={handleSearch}
                        >Enter</button>
                    </form>

```
