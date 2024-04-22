# AssignmentReactjs
//Question 1
function ProductInfo(props){
    
    const {productName,price}=props;
      return(
        <div>
          <h1>Dish:  {productName}</h1>
          <h2>Value: {price}</h2>
        </div>
      )  
}

export default ProductInfo;

//Question2

function WetherMessage(props){

    const {isSunny}=props;
    return(
        <div>
            <h1>Wether</h1>
            <h1>
                { isSunny ? "Its sunny today" : "Its cloudy today"}
            </h1>
        </div>
    )
}

export default WetherMessage;

//Question3

function Employe(props){
    const{name,position,salary}=props;

    return (
        <div>
            <h1>Employe Data</h1>
            <br/>
            <h2>Name : {name}</h2>
            <br/>
            <h3>Position : {position}</h3>
            <br/>
            <h3>Salary : {salary}</h3>
        </div>
    )
}
export default Employe;

// Question4

const ProductList =(props) =>{
    
    return (
        <div>
            <h1>My Product List</h1>
            {props.products.map((item)=> {

                return(
                <p >
                 Name: { item.Name}
                  <br/>
                 Price: {item.price}
                  <br/>
                 Id: {item.id}
                </p>
                )
            })};
        </div>
    )
}

export default ProductList;

return(
   <div class="App">
      <ProductInfo productName="Pasta" price="500"/>*/}
      <WetherMessage isSunny={true}/>
      <Employe name="Ayush" position="Manager" salary="100000"/> 
      <ProductList products = {productList} />
   </div>
)

