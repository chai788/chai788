- 👋 Hi, I’m @chai788
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
chai788/chai788 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->


<dependencies>
        <!-- JUnit -->
        <dependency>
            <groupId>org.junit.jupiter</groupId>
            <artifactId>junit-jupiter</artifactId>
            <version>5.9.3</version>
            <scope>test</scope>
        </dependency>
    </dependencies>

//
    public void testAdd() {
        Addition add1 = new Addition();
        int expectedResult = 10;
        int actualResult = add1.add(5, 2);
        assertEquals(expectedResult, actualResult);
    }

   // dockerfile
   FROM python:3.9-slim
WORKDIR /app
COPY app.py .
RUN pip install flask
EXPOSE 5020
CMD ["python", "app.py"]

// app.py 
from flask import Flask

app = Flask(__name__)

@app.route("/")
def home():
    return "Hello from Docker!"

if __name__ == "__main__":
    app.run(host="0.0.0.0", port=5000)


  
