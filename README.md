# Mc Fleet Date & Ping

![Minecraft](https://img.shields.io/badge/Minecraft-TAB-yellow) ![PlaceholderAPI](https://img.shields.io/badge/PlaceholderAPI-JavaScript-blue)

**Display Date & Ping dynamically on your TAB scoreboard using PlaceholderAPI and Javascript Expansion.**

---

## **Plugins Required**

* [TAB](https://www.spigotmc.org/resources/tab-1-10-1-19.708/)
* [PlaceholderAPI](https://www.spigotmc.org/resources/placeholderapi.6245/)

---

## **Setup Instructions**

### **Step 1: Upload PlaceholderAPI Expansion**

Place the provided expansion file here:

```
plugins/PlaceholderAPI/expansions
```

---

### **Step 2: Reload PlaceholderAPI**

Run the following in console:

```bash
/papi reload
```

**Result:**
A folder named `javascripts` and a file named `javascript_placeholders.yml` will be generated.

---

### **Step 3: Remove Default Files**

Delete the generated folder and file:

```
plugins/PlaceholderAPI/javascripts
plugins/PlaceholderAPI/javascript_placeholders.yml
```

---

### **Step 4: Upload Provided Files**

* Upload the provided files into the same folder.
* Example `javascript_placeholders.yml`:

```yaml
subtime:
  file: subtime.js
  type: string
subping:
  file: subping.js
  type: string
example:
  file: example.js
```

 **All JavaScript files must be in:**
> `plugins/PlaceholderAPI/javascripts/`

For more details: [Javascript Expansion Guide](https://github.com/PlaceholderAPI-Expansions/Javascript-Expansion/wiki)

---

### **Step 5: Unarchive `javascripts.zip`**

* Unarchive the `javascripts.zip` file.
* The `javascripts` folder will reappear.
* Delete the zip file after extraction.

---

### **Step 6: Reload PlaceholderAPI**

```bash
/papi reload
```

---

### **Step 7: Update TAB Configuration**

* Open:

```
plugins/TAB/config.yml
```

* Replace the scoreboard line where you want the date & ping with:

```yaml
' <shadow:#000000FF>&7   %javascript_subtime%  %javascript_subping%'
```

---

### **Step 8: Reload TAB in-game**

```bash
/tab:tab reload
```

---

## **Finished**

You should now see **Date & Ping** on your TAB scoreboard.

---

## **Ping Colors**

| Ping   | Color  |
| ------ | ------ |
| 0–50   | Green  |
| 50–100 | Yellow |
| 100+   | Red    |

---

## **File Structure**

```
plugins/
├─ PlaceholderAPI/
│  ├─ expansions/
│  │  └─ (uploaded expansion file)
│  └─ javascripts/
│     ├─ subtime.js
│     ├─ subping.js
│     └─ example.js
└─ TAB/
   └─ config.yml
```

---

## **Credits**

* JavaScript Expansion: [PlaceholderAPI](https://www.spigotmc.org/resources/placeholderapi.6245/)
* TAB: [TAB Plugin](https://www.spigotmc.org/resources/tab-1-10-1-19.708/)
* AdityaBoii ( OUR CEO ) : <@1236696193556414645>
* ZEROX 
---
