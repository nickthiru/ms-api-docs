# REST API Guidelines  

## URL Structure  

- Use nouns, not verbs, for resource endpoints  
- Use plural nouns for collection resources  
- Use kebab-case for multi-word resource names  
- Use hierarchical structure for related resources  

Examples:  
- GET /flights  
- GET /flights/{id}  
- GET /flights/{id}/seats  
- POST /reservations  

## HTTP Methods  

- GET: Retrieve resources (never modify data)  
- POST: Create new resources  
- PUT: Update resources (entire resource)  
- PATCH: Partial update of resources  
- DELETE: Remove resources  

## Status Codes  

- 200: Success  
- 201: Created  
- 204: No Content (success but no body)  
- 400: Bad Request  
- 401: Unauthorized  
- 403: Forbidden  
- 404: Not Found  
- 500: Internal Server Error  

## Request/Response Format  

- Use JSON for all request and response bodies  
- Use camelCase for JSON property names  
- Include proper Content-Type headers  
- Support filtering, sorting, and pagination for collection endpoints  

## Versioning  

- Include version in URL path: /v1/resource  
- Never remove or change the meaning of fields in an existing API version  
- Add new optional fields to maintain backward compatibility  
