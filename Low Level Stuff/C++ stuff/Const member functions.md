## Const member functions
`cost FooObject object`  - powoduje, iż możemy dostać się tylko do *const* pól oraz funkcji danego obiektu

- *const obiekty* mogą wykorzystywać tylko *const funkcji*, czyli takich które kończą się słowem const:
`int value() const { /* body */}`