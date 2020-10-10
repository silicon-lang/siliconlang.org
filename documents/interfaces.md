# Interfaces

```text
interface Name {
    first: string;
    last: string;
}

interface Person {
    name: Name;
    age: i32;
}

interface WithLicense {
    licensed: bool;
}

interface Doctor extends Person, WithLicense {
    field: string;
}
```

