public class Product{
    String pcode;
    String pname;
    int price;
    public Product(String pcode_get,String pname_get,int price_get){
        pcode=pcode_get;
        pname=pname_get;
        price=price_get;

    }
    public int get_price(){
        return price;

    }



public static void main(String args[]) {
    Product p1 = new Product("a123", "TV", 2);
    Product p2 = new Product("b123", "radio", 21);
    Product p3 = new Product("c123", "dvd", 3);
    if (p1.price <= p3.price && p1.price <= p2.price)
        System.out.println("lowest product ID is:" + p1.pcode);
    if (p3.price <= p1.price && p3.price <= p2.price)
        System.out.println("lowest product ID is:" + p3.pcode);
    if (p2.price <= p3.price && p2.price <= p1.price)
        System.out.println("lowest product ID is:" + p2.pcode);
}
}



