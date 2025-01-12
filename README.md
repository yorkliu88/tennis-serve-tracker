# tennis-serve-tracker

Google Sheet, App Script, after modify App Scrip Code, need manage deployment
Click Pencil, add new Version, give a description, and save it, then archive the code one

CORS issue was resolved by adding below mode no-cors in github code when do POST

                const response = await fetch("https://script.google.com/macros/s/AKfycbyWJ2UAib1Vliq9OonS6unfqiBfsmRBDmrvPZTBmN0MOwP_yPr65ZgJac_m2lv0RRTu/exec", {
                    mode: "no-cors",
                    method: "POST",
                    headers: { "Content-Type": "application/json" },
                    body: JSON.stringify(sessionData),
                });
