![alt text](<demand fulfillment strategies .png>)

The image compares **four fulfillment strategies** used in manufacturing and supply chains:

**MTS → ATO → MTO → ETO**

As you move from left to right, the product becomes **more customized**, the lead time becomes **longer**, and inventory risk usually becomes **lower**.

---

## 1. Make-to-Stock, MTS

**Meaning:**
The company produces finished goods **before receiving customer orders**. Products are made based on forecasts and stored as inventory.

**Simple idea:**
“Produce first, sell later.”

**How it works:**

A company predicts demand, manufactures finished products in bulk, stores them in warehouses or retail shelves, and ships immediately when customers buy.

**Real-world examples:**

Supermarkets use MTS for products like bottled water, rice, biscuits, soap, toothpaste, and canned food. These are standard products with predictable demand.

Electronics retailers may stock common TV models, mobile accessories, or household appliances before customers order them.

**Supply chain characteristics:**

MTS has the **shortest customer lead time** because the product is already finished. The customer can buy it immediately.

The downside is **high inventory risk**. If the forecast is wrong, the company may end up with excess stock, obsolete inventory, markdowns, or waste.

**Best used when:**

Demand is predictable, products are standardized, customers expect quick availability, and unit cost can be reduced through mass production.

**Example from ERP perspective:**

In SAP or Oracle ERP, MTS usually depends heavily on demand forecasting, MRP runs, safety stock, reorder points, and finished goods inventory planning.

---

## 2. Assemble-to-Order, ATO

**Meaning:**
The company produces or stocks standard components in advance, but the final product is assembled only after receiving a customer order.

**Simple idea:**
“Prepare modules first, assemble after order.”

**How it works:**

The company keeps semi-finished parts, modules, or subassemblies ready. When the customer places an order, the final configuration is assembled quickly.

**Real-world examples:**

Dell computers are a classic ATO example. Dell may keep processors, RAM, SSDs, screens, and cases available. When a customer selects a configuration, the final laptop or desktop is assembled.

Subway is another simple example. Bread, vegetables, sauces, and fillings are prepared in advance, but the sandwich is assembled after the customer chooses the combination.

Automotive companies may use ATO for vehicles where customers choose color, engine type, wheels, or interior packages from predefined options.

**Supply chain characteristics:**

ATO offers **moderate customization** with relatively short lead time. It is a balance between MTS efficiency and MTO flexibility.

Inventory risk is lower than MTS because the company stocks components instead of finished products. The same component can be used in multiple final products.

**Best used when:**

Products are modular, customers want choices, and the company can standardize components while still offering variety.

**Example from ERP perspective:**

ATO often uses configurable BOMs, variant configuration, component availability checks, and final assembly orders triggered by sales orders.

---

## 3. Make-to-Order, MTO

**Meaning:**
The company starts manufacturing the product only after receiving a confirmed customer order.

**Simple idea:**
“Order first, manufacture later.”

**How it works:**

The company may keep raw materials or common materials in stock, but actual production begins only after a customer places an order.

**Real-world examples:**

A custom furniture company may not build a dining table until the customer selects the size, wood type, finish, and design.

Tailored clothing is another example. The fabric may be available, but the shirt or suit is made after taking the customer’s measurements.

Industrial spare parts, specialized tools, custom machinery parts, and made-to-measure packaging often follow MTO.

**Supply chain characteristics:**

MTO provides **high customization**, but the customer must wait longer because manufacturing happens after the order.

Inventory risk is lower than MTS because the company does not hold many finished goods. However, production planning becomes more complex because each order may be different.

**Best used when:**

Demand is uncertain, finished goods are expensive to stock, products require customer-specific features, or customers are willing to wait.

**Example from ERP perspective:**

MTO usually links the sales order directly to production. In ERP, this may involve sales-order-specific planning, production orders, pegged requirements, and customer-specific costing.

---

## 4. Engineer-to-Order, ETO

**Meaning:**
The company designs and engineers the product only after receiving the customer order. The product may not exist yet in final form.

**Simple idea:**
“Design first, then build for one customer.”

**How it works:**

The customer gives requirements. Engineering teams create drawings, specifications, BOMs, routings, and project plans. Procurement and production happen after the design is approved.

**Real-world examples:**

Large construction projects are ETO. A bridge, airport terminal, factory, or skyscraper is designed for a specific site and customer.

Aerospace and defense projects often use ETO because each aircraft system, satellite component, or defense platform may require unique engineering.

Shipbuilding, heavy industrial machinery, power plants, and custom automation lines are also strong ETO examples.

**Supply chain characteristics:**

ETO has the **highest customization** and usually the **longest lead time**. There is little or no finished goods inventory risk because the product is built for a specific customer.

The main risks are engineering delays, design changes, cost overruns, procurement delays, and project complexity.

**Best used when:**

The product is unique, expensive, technically complex, and customer-specific.

**Example from ERP perspective:**

ETO often requires integration between PLM, CAD, project systems, procurement, manufacturing, and finance. BOMs may evolve during the project, and change management becomes critical.

---

## The Key Concept: Customer Order Decoupling Point

The **Customer Order Decoupling Point**, or CODP, is the point in the supply chain where the process switches from forecast-driven to order-driven.

Before the CODP, activities are based on forecast.
After the CODP, activities are based on actual customer orders.

In simple terms:

| Strategy | What is ready before order?     | What happens after order?        |
| -------- | ------------------------------- | -------------------------------- |
| MTS      | Finished goods                  | Pick, pack, ship                 |
| ATO      | Components/modules              | Final assembly                   |
| MTO      | Raw materials/basic inputs      | Manufacture product              |
| ETO      | Design capability/supplier base | Design, engineer, procure, build |

---

## Quick Comparison

| Strategy | Customization |       Lead Time |               Inventory Risk | Example                                              |
| -------- | ------------: | --------------: | ---------------------------: | ---------------------------------------------------- |
| MTS      |           Low |      Very short |                         High | Grocery items, standard appliances                   |
| ATO      |        Medium | Short to medium |                       Medium | Dell PC, Subway sandwich                             |
| MTO      |          High |            Long |                          Low | Custom furniture, tailored clothing                  |
| ETO      |     Very high |       Very long | Very low finished-goods risk | Construction, aerospace, custom industrial equipment |

---

## Practical Supply Chain Interpretation

Use **MTS** when demand is stable and speed matters.

Use **ATO** when customers want options but the company still wants efficiency.

Use **MTO** when customers want customized products and are willing to wait.

Use **ETO** when every order is a unique project requiring design and engineering.

For your supply chain/ERP lens, the main difference is where the system creates demand signals: forecast drives MTS, sales-order configuration drives ATO, sales-order production drives MTO, and project/design approval drives ETO.
