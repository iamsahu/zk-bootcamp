- Decorators
    - #[contract]: Specifies that it is a cairo contract and not a program
    - #[event]: Used to define an event
    - Function decorators
        - #[external]
        - #[view]
        - #[constructor]
        - #[l1_handler]: less common, but shows that the function can receive a message from L1
- Storing data
    - Have states maintained by the starknetOS
    - use a struct `Storage` and withing that specify the variables that you want to store
    ``` 
    struct Storage {
        contract_index: u8,
        balances: LegacyMap::<ContractAddress, u256>
    }
    ```
    - Reading from storage
        - contract_index::read();
    - Writing to storage
        - contract_index::write(index);
    ```
    #[view]
    fn get_contract_index() -> u8 {
        contract_index::read()
    }
    ```
- Importing other contracts
    - Contract class
    - Contract instance
- Account abstraction