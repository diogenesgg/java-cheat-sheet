# java-cheat-sheet
My Notes on Java

## Deprecated Classes/APIs
 - SimpleDateFormat
 - java.util.Date
 - java.util.HashTable
   - Not officially deprecated (with the @Deprecated). However, it is widely considered obsolete, and its use is discouraged for new development.
   - Use HashMap or ConcurrentHashMap instead.

## Multithreading
 - volatile:
   - "This variable changes a lot, and is accessed by multiple threads! Don't cache it at the CPU level (registers, cache), only have it in memory."
 - synchronized:
   - When applied to multiple methods, one method being accessed blocks the other synchronized ones! 

## Spring Boot 

