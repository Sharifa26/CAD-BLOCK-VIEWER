<h1 align="center">🧱 CAD Block Viewer</h1>

<p align="center">
  A full-stack application to upload, parse, and view CAD `.dxf` files. Extracts blocks/entities like INSERT and SPLINE, saves them into a PostgreSQL database, and displays them in a clean, searchable frontend interface.
</p>

<p align="center">
  <a href="#setup">Setup Instructions</a> • 
  <a href="#libraries">Library Choices</a> • 
  <a href="#challenges">Challenges</a> • 
  <a href="#ai">Use of AI Coding Assistants</a>
</p>

---

## 🔧 <a id="setup">Setup Instructions</a>


<h3> 💻Backend Repository</h3>

https://github.com/Sharifa26/CAD-Block-Viewer-Backend

where you can the backend repository setup instructions,Installation and Configuration , Database Schema and API Documentation.


<h3> 💻Frontend Repository</h3>

https://github.com/Sharifa26/CAD-Block-Viewer-Frontend

where you can the Find  frontend repository setup instructions, and how to run the project.

## <a id="libraries">📚 Libraries Used</a>

### 🧠 Backend

- **Express.js**: Lightweight, minimal, and perfect for creating REST APIs.
- **Multer**: Simplifies file uploads; supports file filtering and limits.
- **pg**: Direct PostgreSQL driver for flexibility in query control.
- **dotenv**: Manage credentials and environment configs easily.
- **cors**: Enable cross-origin requests from frontend during development.

### 🎨 Frontend

- **React**: Ideal for dynamic UI and state-based updates.
- **Tailwind CSS**: Fast prototyping and elegant design system.
- **Fetch API**: Simple and effective for API communication without external libraries.




## <a id="challenges">📝 Challenges</a>

| Challenge                          | Solution                                                                                      |
|-----------------------------------|-----------------------------------------------------------------------------------------------|
| **Parsing `.dxf` Files**           | DXF parsing required identifying correct libraries and understanding the INSERT/SPLINE structure. I explored multiple packages and tested outputs before finalizing the logic. |
| **Coordinate Normalization**       | Not all DXF files used the same coordinate origins. I wrote logic to normalize these during processing. |
| **Asynchronous File Parsing**      | Handling parsing in sequence while maintaining responsiveness involved wrapping the file handling logic in async/await blocks. |
| **Frontend Pagination & Filtering**| Managed this using internal React state and conditionals. Will optimize further with lazy loading. |
| **Expandable Block Details**       | Implemented toggled sections in React with smooth transitions and conditional rendering.      |

---

## <a id="ai">🤖 Use of AI Coding Assistants</a>

AI coding assistants (like ChatGPT and GitHub Copilot) were instrumental in:
- Drafting logic for parsing DXF blocks and handling JSON data structures.
- Speeding up iteration by helping debug errors and suggesting improvements.

<p align="center">Made with ❤️ by Sharifa26</p>
