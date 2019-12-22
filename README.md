# redux-counter-
my very first redux project
const INCREMENT = 'INCREMENT'; 
const DECREMENT = 'DECREMENT'; 

const counterReducer =(state=0, action) =>{
    switch(action.type) {
         case INCREMENT:
            return (state += 1)
            

        case DECREMENT:
            return (state -= 1)

    default:
        return state 
    }
}
    let count = 0
const incAction = () => {
    return{
        type: INCREMENT
    }
}

const decAction = () => {
    return {
        type: DECREMENT
    }
}

const store = Redux.createStore(counterReducer)
