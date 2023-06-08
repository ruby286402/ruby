import speedtest

# 创建一个Speedtest对象
st speedtest.Speedtest()

# 获取下载速度、上传速度和延迟
download_speed = st.download() / 1000000
upload_speed = st.upload() / 1000000
ping = st.results.ping

# 打印下载速度、上传速度和延迟
print("Download speed: {:.2f} Mbps".format(download_speed))
print("Upload speed: {:.2f}".format(upload_speed))
print("Ping: {:.2f} ms".format(ping))
