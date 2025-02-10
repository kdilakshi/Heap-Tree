# Heap-Tree
max heap, min heap


/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 * Click nbfs://nbhost/SystemFileSystem/Templates/Classes/Main.java to edit this template
 */
package trees;

/**
 *
 * @author dilakshi
 */import java.util.PriorityQueue;
import java.util.Collections;

public class heaptree {
    public static void main(String[] args) {
        // Max Heap using PriorityQueue (Reverse Order)
        PriorityQueue<Integer> maxHeap = new PriorityQueue<>(Collections.reverseOrder());

        // Insert elements
        int[] elements = {30, 12, 70, 44, 55, 15};
        for (int num : elements) {
            maxHeap.add(num);
            System.out.println("Inserted: " + num + " | Max Heap: " + maxHeap);
        }

        // Remove elements (Max Heap Property)
        System.out.println("\nRemoving elements:");
        while (!maxHeap.isEmpty()) {
            System.out.println("Removed: " + maxHeap.poll() + " | Remaining: " + maxHeap);
        }
    }
    
    
public class MinHeapExample {
    public static void main(String[] args) {
        // Min Heap using PriorityQueue
        PriorityQueue<Integer> minHeap = new PriorityQueue<>();

        // Insert elements
        int[] elements = {30, 12, 70, 44, 55, 15};
        for (int num : elements) {
            minHeap.add(num);
            System.out.println("Inserted: " + num + " | Min Heap: " + minHeap);
        }

        // Remove elements (Min Heap Property)
        System.out.println("\nRemoving elements:");
        while (!minHeap.isEmpty()) {
            System.out.println("Removed: " + minHeap.poll() + " | Remaining: " + minHeap);
        }
    }
}
}

