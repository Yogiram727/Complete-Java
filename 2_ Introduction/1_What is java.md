# Java Notes

## What is Java?
- Java is a programming language and a platform.
- It is high-level, robust, object-oriented, and secure.
- Developed by Sun Microsystems (now a subsidiary of Oracle) in 1995.
- James Gosling is known as the father of Java.
- Originally named Oak, but changed to Java due to a trademark issue.

## Platform
- A platform is any hardware or software environment where a program runs.
- Java is considered a platform because it has a runtime environment (JRE) and API.

## Java Example
```java
class Simple{  
    public static void main(String args[]){  
        System.out.println("Hello Java");  
    }  
}
```
# Application of Java

- Java is used in over 3 billion devices worldwide.
- Common areas where Java is used:
  - **Desktop Applications**: Acrobat Reader, media player, antivirus, etc.
  - **Web Applications**: irctc.co.in, javatpoint.com, etc.
  - **Enterprise Applications**: Banking applications and large-scale distributed systems.
  - **Mobile Applications**: Android apps and Java ME.
  - **Embedded Systems**: Devices like TVs, microwaves, and other embedded systems.
  - **Smart Cards**: Used in various industries, including banking and telecommunication.
  - **Robotics**: Control systems and automation using Java.
  - **Games**: Java is also used in developing 2D and 3D games.

# Types of Java Applications

1. **Standalone Application**
   - Also known as desktop or window-based applications.
   - Traditional software that needs to be installed on each machine.
   - Examples: Media players, antivirus software.
   - Technologies used: AWT and Swing for creating standalone applications.

2. **Web Application**
   - Runs on the server-side and generates dynamic web pages.
   - Java web applications can be found in online systems like irctc.co.in.
   - Technologies used: Servlet, JSP, Struts, Spring, Hibernate, JSF, etc.

3. **Enterprise Application**
   - Distributed applications that are used by large organizations, such as banking systems.
   - Advantages: High security, load balancing, clustering.
   - Technologies used: Enterprise Java Beans (EJB) and other enterprise-focused frameworks.

4. **Mobile Application**
   - Java is widely used for creating mobile applications.
   - Technologies used: Android (based on Java) and Java ME (Micro Edition) for mobile development.

# Difference Between Java Editions

## 1. Java SE (Standard Edition)
- **Purpose**: Core platform for general-purpose programming.
- **Used for**:
  - Building desktop applications and basic standalone programs.
  - Learning fundamental Java programming concepts.
- **APIs**: 
  - `java.lang` (core language features),
  - `java.util` (data structures, collections),
  - `java.io` (input/output operations),
  - `java.net` (networking),
  - `java.sql` (database connectivity),
  - GUI libraries like AWT and Swing.
  
**Example Use**:
- Simple desktop applications (media players, calculators).
- Command-line utilities.
- Learning and practicing Java programming concepts.

---

## 2. Java EE (Enterprise Edition)
- **Purpose**: Framework for building large-scale, distributed, and web-based applications.
- **Used for**:
  - Developing enterprise-level applications that require security, scalability, and reliability.
  - Web-based applications, cloud applications, and large distributed systems.
- **APIs**:
  - Servlets, JSP (for web applications),
  - EJB (for large-scale enterprise applications),
  - Web Services (for service-oriented architectures),
  - JPA (for database handling).
  
**Example Use**:
- Banking systems, e-commerce platforms, and enterprise resource planning (ERP) systems.
- Complex web applications (online booking systems, enterprise portals).

---

## 3. Java ME (Micro Edition)
- **Purpose**: Targeted for mobile and embedded devices with limited resources (memory, processing power).
- **Used for**:
  - Developing applications for resource-constrained devices such as mobile phones, PDAs, and embedded systems (TVs, washing machines, etc.).
- **APIs**:
  - Scaled-down versions of standard Java libraries, optimized for small devices.
  - APIs for handling user interfaces and networking specific to mobile devices.

**Example Use**:
- Java-based mobile applications for feature phones.
- Applications in embedded systems such as set-top boxes and IoT devices.

---

## 4. JavaFX
- **Purpose**: Platform for building rich internet applications (RIAs) with modern, lightweight graphical user interfaces.
- **Used for**:
  - Developing visually rich desktop and web applications with advanced UI elements.
  - GUI applications that require rich media content like animations, video, and audio.
- **APIs**:
  - JavaFX has its own user interface libraries for building sophisticated UIs.
  - Support for 2D and 3D graphics, video playback, and embedded web content.

**Example Use**:
- Media-rich desktop applications (video editing software, interactive dashboards).
- Web-based applications with modern, dynamic user interfaces.

---

## Summary of Differences:
- **Java SE**: Core Java for general-purpose programming.
- **Java EE**: Focuses on enterprise and large-scale web applications.
- **Java ME**: Optimized for mobile and embedded devices with limited resources.
- **JavaFX**: Specializes in building rich, interactive user interfaces for desktop and web applications.
