<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AI Assistant Widget</title>

    <!-- === بداية كود التصميم (CSS) === -->
    <style>
        /* تصميم أيقونة الـ Widget */
        #widget-icon {
            position: fixed;
            bottom: 20px;
            right: 20px;
            background-color: #007bff;
            color: white;
            width: 60px;
            height: 60px;
            border-radius: 50%;
            display: flex;
            justify-content: center;
            align-items: center;
            cursor: pointer;
            box-shadow: 0 4px 8px rgba(0,0,0,0.2);
            z-index: 9998;
            transition: transform 0.2s;
        }

        #widget-icon:hover {
            transform: scale(1.1);
        }

        /* تصميم نافذة المحادثة */
        #chat-window {
            position: fixed;
            bottom: 100px;
            right: 20px;
            width: 350px;
            max-width: 90%;
            height: 500px;
            max-height: 80vh;
            background-color: white;
            border-radius: 15px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.3);
            display: flex;
            flex-direction: column;
            overflow: hidden;
            z-index: 9999;
            transition: opacity 0.3s, transform 0.3s;
            transform-origin: bottom right;
        }

        /* لإخفاء النافذة */
        .hidden {
            opacity: 0;
            transform: scale(0.5);
            pointer-events: none;
        }

        /* تصميم رأس النافذة */
        #chat-header {
            background-color: #007bff;
            color: white;
            padding: 15px;
            font-weight: bold;
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-shrink: 0;
        }

        #close-btn {
            background: none;
            border: none;
            color: white;
            font-size: 24px;
            cursor: pointer;
        }

        /* تصميم جسم المحادثة */
        #chat-body {
            flex-grow: 1;
            padding: 15px;
            overflow-y: auto;
            background-color: #f4f4f4;
            display: flex;
            flex-direction: column;
        }

        .message {
            padding: 10px 15px;
            border-radius: 20px;
            margin-bottom: 10px;
            max-width: 80%;
            line-height: 1.4;
        }

        .user {
            background-color: #007bff;
            color: white;
            align-self: flex-end;
            border-bottom-right-radius: 5px;
        }

        .bot {
            background-color: #e9e9eb;
            color: black;
            align-self: flex-start;
            border-bottom-left-radius: 5px;
        }

        /* تصميم جزء الإدخال */
        #chat-footer {
            display: flex;
            padding: 10px;
            border-top: 1px solid #ddd;
            background-color: #fff;
            flex-shrink: 0;
        }

        #user-input {
            flex-grow: 1;
            border: 1px solid #ccc;
            border-radius: 20px;
            padding: 10px 15px;
            margin-left: 10px;
            font-family: inherit;
            font-size: 16px;
        }

        #send-btn {
            background-color: #007bff;
            color: white;
            border: none;
            border-radius: 50%;
            width: 45px;
            height: 45px;
            cursor: pointer;
            display: flex;
            justify-content: center;
            align-items: center;
            transition: background-color 0.2s;
        }
        #send-btn:hover {
            background-color: #0056b3;
        }
    </style>
    <!-- === نهاية كود التصميم (CSS) === -->
</head>
<body>

    <!-- === بداية هيكل الـ Widget (HTML) === -->
    <!-- الأيقونة التي تظهر في زاوية الشاشة -->
    <div id="widget-icon">
        <svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" fill="currentColor" viewBox="0 0 16 16">
            <path d="M8.5 1.866a1 1 0 1 0-1 0V3h-2A4.5 4.5 0 0 0 1 7.5V8a1 1 0 0 0-1 1v2a1 1 0 0 0 1 1v.5A4.5 4.5 0 0 0 5.5 17h5a4.5 4.5 0 0 0 4.5-4.5v-.5a1 1 0 0 0 1-1v-2a1 1 0 0 0-1-1V7.5A4.5 4.5 0 0 0 10.5 3h-2zM14 7.5V13a5.5 5.5 0 0 1-5.5 5.5h-1A5.5 5.5 0 0 1 2 13V7.5a3.5 3.5 0 0 1 3.5-3.5h1a3.5 3.5 0 0 1 3.5 3.5Z"/>
            <path d="M6 12.5a.5.5 0 0 1 .5-.5h3a.5.5 0 0 1 0 1h-3a.5.5 0 0 1-.5-.5M3 8.062C3 6.76 4.235 5.765 5.53 5.886a26.6 26.6 0 0 0 4.94 0C11.765 5.765 13 6.76 13 8.062v1.157a.93.93 0 0 1-.765.935c-.845.147-2.34.346-4.235.346s-3.39-.2-4.235-.346A.93.93 0 0 1 3 9.219zm0 1.572V11.5a.5.5 0 0 0 .5.5h9a.5.5 0 0 0 .5-.5V9.634c.898.173 1.998.386 3.008.42a.5.5 0 0 0 .492-.498v-1.1a.5.5 0 0 0-.492-.498c-1.01-.034-2.11-.247-3.008-.42V4.5a.5.5 0 0 0-.5-.5h-9a.5.5 0 0 0-.5.5v1.634c-.898-.173-1.998-.386-3.008-.42a.5.5 0 0 0-.492.498v1.1a.5.5 0 0 0 .492.498c1.01.034 2.11.247 3.008.42z"/>
        </svg>
    </div>

    <!-- نافذة المحادثة (مخفية في البداية ) -->
    <div id="chat-window" class="hidden">
        <div id="chat-header">
            <span>مساعدك الذكي</span>
            <button id="close-btn">&times;</button>
        </div>
        <div id="chat-body">
            <div class="message bot">مرحباً! كيف يمكنني مساعدتك اليوم؟</div>
        </div>
        <div id="chat-footer">
            <input type="text" id="user-input" placeholder="اكتب رسالتك هنا...">
            <button id="send-btn">
                <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" fill="currentColor" viewBox="0 0 16 16">
                    <path d="M15.854.146a.5.5 0 0 1 .11.54l-5.819 14.547a.75.75 0 0 1-1.329.124l-3.178-4.995L.643 7.184a.75.75 0 0 1 .124-1.33L15.314.037a.5.5 0 0 1 .54.11ZM6.636 10.07l2.761 4.338L14.13 2.576zm6.787-8.201L1.591 6.602l4.339 2.76z"/>
                </svg>
            </button>
        </div>
    </div>
    <!-- === نهاية هيكل الـ Widget (HTML ) === -->


    <!-- === بداية كود التشغيل (JavaScript) === -->
    <script>
        document.addEventListener('DOMContentLoaded', function() {
            // تعريف العناصر
            const widgetIcon = document.getElementById('widget-icon');
            const chatWindow = document.getElementById('chat-window');
            const closeBtn = document.getElementById('close-btn');
            const sendBtn = document.getElementById('send-btn');
            const userInput = document.getElementById('user-input');
            const chatBody = document.getElementById('chat-body');

            // =================================================================
            // ==   مهم جداً: ضع رابط الويب هوك الخاص بك من n8n هنا          ==
            // =================================================================
            const N8N_WEBHOOK_URL = 'https://example.com/webhook/your-n8n-webhook-id';

            // إظهار وإخفاء نافذة المحادثة
            widgetIcon.addEventListener('click', ( ) => {
                chatWindow.classList.toggle('hidden');
                if (!chatWindow.classList.contains('hidden')) {
                    userInput.focus();
                }
            });

            closeBtn.addEventListener('click', () => {
                chatWindow.classList.add('hidden');
            });

            // إرسال الرسالة عند الضغط على زر الإرسال
            sendBtn.addEventListener('click', sendMessage);

            // إرسال الرسالة عند الضغط على Enter
            userInput.addEventListener('keypress', function(e) {
                if (e.key === 'Enter') {
                    sendMessage();
                }
            });

            // دالة لإرسال الرسالة
            function sendMessage() {
                const messageText = userInput.value.trim();
                if (messageText === '') return;

                // 1. عرض رسالة المستخدم على الشاشة
                addMessage(messageText, 'user');
                userInput.value = '';
                userInput.disabled = true; // تعطيل الإدخال أثناء انتظار الرد
                addTypingIndicator(); // إضافة مؤشر "يكتب الآن"

                // 2. إرسال الرسالة إلى n8n
                fetch(N8N_WEBHOOK_URL, {
                    method: 'POST',
                    headers: {
                        'Content-Type': 'application/json',
                    },
                    body: JSON.stringify({ message: messageText })
                })
                .then(response => {
                    if (!response.ok) {
                        throw new Error('Network response was not ok');
                    }
                    return response.json();
                })
                .then(data => {
                    removeTypingIndicator(); // إزالة مؤشر "يكتب الآن"
                    // 3. عرض رد n8n (الروبوت) على الشاشة
                    // نفترض أن n8n يعيد الرد في حقل اسمه "reply"
                    const botReply = data.reply || 'عذراً، لم أتمكن من معالجة طلبك.';
                    addMessage(botReply, 'bot');
                })
                .catch(error => {
                    console.error('Error:', error);
                    removeTypingIndicator();
                    addMessage('حدث خطأ أثناء الاتصال بالخادم. يرجى المحاولة مرة أخرى.', 'bot');
                })
                .finally(() => {
                    userInput.disabled = false; // إعادة تفعيل الإدخال
                    userInput.focus();
                });
            }

            // دالة لإضافة رسالة إلى واجهة المحادثة
            function addMessage(text, type) {
                const messageElement = document.createElement('div');
                messageElement.classList.add('message', type);
                messageElement.textContent = text;
                chatBody.appendChild(messageElement);
                // تمرير الشاشة للأسفل لرؤية آخر رسالة
                chatBody.scrollTop = chatBody.scrollHeight;
            }
            
            // دالة لإضافة مؤشر الكتابة
            function addTypingIndicator() {
                const typingIndicator = document.createElement('div');
                typingIndicator.classList.add('message', 'bot', 'typing-indicator');
                typingIndicator.innerHTML = '<span>.</span><span>.</span><span>.</span>';
                chatBody.appendChild(typingIndicator);
                chatBody.scrollTop = chatBody.scrollHeight;
            }

            // دالة لإزالة مؤشر الكتابة
            function removeTypingIndicator() {
                const indicator = document.querySelector('.typing-indicator');
                if (indicator) {
                    indicator.remove();
                }
            }
        });
    </script>
    <!-- === نهاية كود التشغيل (JavaScript) === -->

</body>
</html>
