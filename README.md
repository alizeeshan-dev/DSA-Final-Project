# Mini Food-Delivery Simulator

**Team Members:**

- Ali Zeeshan (24K-0749)
- Hasan Khan (24K-0525)
- Zaid Amir (24K-0813)

**Course:** Data Structures  
**Instructor:** Ms. Fizza Aqeel  
**Date:** 9/10/25

## Overview

A console-based food delivery simulator built in C++ that demonstrates the use of various data structures including Linked Lists, Queues, Stacks, Binary Search Trees, Priority Queues, and Graphs with Dijkstra's Algorithm. Set in Karachi, Pakistan with real street names and locations.

> **Note:** The project runs directly from source code (`project.cpp`). No permanent exe files are kept in the repository.

## Features

✅ CSV auto-loading for nodes/edges, restaurants, and agents  
✅ Dynamic user creation on order placement  
✅ Dispatcher with Priority Queue for urgent orders and FIFO Queue for backlog  
✅ Shortest-path routing via Dijkstra's Algorithm with path visualization  
✅ Separate distance (km) and ETA (minutes) calculations  
✅ Undo last assignment using Stack  
✅ Order history stored in Linked List  
✅ BST for restaurant search by name  
✅ ASCII network map visualization with restaurant indicators

## File Structure

```
project.cpp           - Main implementation
nodes.csv            - Graph nodes
edges.csv            - Graph edges (source, destination, weight)
restaurants.csv      - Restaurant data (id, name, nodeId)
users.csv            - User data (id, name, nodeId)
agents.csv           - Delivery agent data (id, name, nodeId)
```

## Key Implementation Details

1. **Agent Selection:** Uses Dijkstra to find nearest available agent from restaurant location
2. **ETA Calculation:** Computes shortest path from restaurant to user
3. **Order Priority:** Priority ≥5 goes to urgent queue, <5 goes to backlog
4. **Undo Functionality:** Stack stores last assignment for reversal
5. **Order Tracking:** Linked list maintains complete order history

## Future Enhancements

- Real-time order tracking
- Agent completion and availability reset
- Multi-order assignment per agent
- Advanced routing with traffic simulation
- GUI interface

---

**Developed as part of Data Structures course final project**
