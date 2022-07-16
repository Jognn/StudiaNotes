## Reference vs Pointer

`int foobar(int *var)` - pointer
`int foobar(int &var)` - referencja

- Referencja (&) zapewnia, że *var* nie jest nullem

**Poniższy zapis również jest poprawny:**
`int *foobar()`
`int &foobar()`