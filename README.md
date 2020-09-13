# Book

import java.lang.*;
public class Book {
    private String edition;
    private int pages;

    public Book(String n, int a){
        edition = n;
        pages = a;
    }

    public Book(String n) {
        edition = n;
        pages = 0;
    }
    public Book() {
        edition = "Audio format";
        pages = 0;
    }
    public void setPages (int pages){
        this.pages = pages;
    }
    public void setEdition (String edition){
        this.edition = edition;
    }
    public String getEdition (String edition){
        return edition;
    }
    public int getPages() {
        return pages;
    }
    public String toString(){
        return this.edition+", size "+this.pages;
    }
}

import java.lang.*;
    public class TestBook {
        public static void main(String[] args) {
            Book d1 = new Book("Феникс", 214);
            Book d2 = new Book("Эксмо - Аст", 756);
            Book d3 = new Book("Фламинго", 512);
            d3.setPages(1);
            System.out.println(d1);
        }

    }
