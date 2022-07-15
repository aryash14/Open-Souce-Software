# Check 1:

<img width="863" alt="image" src="https://user-images.githubusercontent.com/71746459/179249715-04e0b287-3f5e-423c-bb85-6b7b62352282.png">

# Check 2:

Find the Nightly and Experimental sections and look at some of the submissions. How can you see what tests were run for a particular submission?
- Number of Not run + Fail + Pass would be the number of tests ran.
Find a submission with errors. Can you see what the error condition was? How does this help you debug the failure?
Yes the error is with a  file not being found in our case this file is openssl/opensslconf.h and the error is fatal error: openssl/opensslconf.h: No such file or directory
And when the code hits #include <openssl/opensslconf.h> it terminates the compilation
Find a system that is close to your specific configuration in the Nightly, Nightly Expected or one of the Masters sections. How clean is the dashboard? Are there any errors that you need to be concerned with?
Dashbord shows how many tests failed and how any passes. We can also see errors and warning there are.

No erros with my submission. Which was consistent with programs that had the same structure as mine.

<img width="1415" alt="image" src="https://user-images.githubusercontent.com/71746459/179254177-f1f51aea-d066-4e00-a0f4-f8e24b714820.png">

<img width="1440" alt="image" src="https://user-images.githubusercontent.com/71746459/179254222-38116d94-7b65-406b-993d-ad7e9880baa1.png">

# Check 3:
