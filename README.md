﻿# DS-Orienta-oObjetos

 import java.util.*;
public class EntradaComScanner { //metodo principal

    public static void main(String[] args) {
        float largura, comprimento, area, perimetro;
        Scanner sc;
        try {
            System.out.println("entre com o comprimento: ");
            sc = new Scanner(System.in);
            comprimento = sc.nextFloat();

            System.out.println("entre com a largura: ");
            sc = new Scanner(System.in);
            largura = sc.nextFloat();

            area = comprimento * largura;
            perimetro = comprimento * 2 + largura * 2;

            System.out.println("Area do terreno: " + area);
            System.out.println("Area do perimetro: " + perimetro);
        }
        catch (NumberFormatException e) {
            System.out.println("houve erro na conversao, digite apenas caracteres numericos!");
        }
    }
}
