FROM alpine        
# взять базовый образ alpine
RUN apk add --update --no-cache curl wget busybox-extras netcat-openbsd py3-pip bash && \      
    pip install awscli                  
    # установка консоли для работы с амазоном
RUN apk --purge -v del py-pip           
# удаляет установденный py-pip для оптимизации образа 
CMD tail -f /dev/null                   
# просто команда, которая не дает образу сразу умереть после окончания процессов
