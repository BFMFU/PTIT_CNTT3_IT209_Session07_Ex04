root@azvps-dynamic:~# sudo nano /etc/nginx/sites-enabled/spring-proxy.conf
root@azvps-dynamic:~# sudo systemctl reload nginx
root@azvps-dynamic:~# nginx -t
nginx: the configuration file /etc/nginx/nginx.conf syntax is ok
nginx: configuration file /etc/nginx/nginx.conf test is successful
root@azvps-dynamic:~# curl http://localhost/
<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Thông tin học viên</title>

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: Arial, sans-serif;
            background: #f2f4f7;
            color: #333;
            min-height: 100vh;

            display: flex;
            justify-content: center;
            align-items: center;
        }

        .student-card {
            width: 500px;
            background: white;
            border-radius: 12px;
            padding: 30px;
            box-shadow: 0 5px 20px rgba(0, 0, 0, 0.1);
        }

        .title {
            text-align: center;
            margin-bottom: 25px;
            color: #2c3e50;
        }

        .avatar {
            width: 100px;
            height: 100px;
            border-radius: 50%;
            background: #3498db;
            color: white;

            display: flex;
            justify-content: center;
            align-items: center;

            font-size: 36px;
            font-weight: bold;

            margin: 0 auto 20px;
        }

        .student-name {
            text-align: center;
            font-size: 24px;
            margin-bottom: 25px;
            color: #222;
        }

        .info {
            border-top: 1px solid #eee;
        }

        .info-row {
            display: flex;
            padding: 12px 0;
            border-bottom: 1px solid #eee;
        }

        .label {
            width: 150px;
            font-weight: bold;
            color: #555;
        }

        .value {
            flex: 1;
            color: #333;
        }

        .status {
            display: inline-block;
            padding: 5px 12px;
            border-radius: 20px;
            background: #d4edda;
            color: #155724;
            font-size: 14px;
            font-weight: bold;
        }
    </style>
</head>

<body>

    <div class="student-card">

        <h1 class="title">THÔNG TIN HỌC VIÊN</h1>

        <div class="avatar">
            NM
        </div>

        <h2 class="student-name">
            Nguyễn Duy Mạnh
        </h2>

        <div class="info">

            <div class="info-row">
                <div class="label">Mã học viên:</div>
                <div class="value">HV001</div>
            </div>

            <div class="info-row">
                <div class="label">Lớp:</div>
                <div class="value">HN_KS24_CNTT3</div>
            </div>

            <div class="info-row">
                <div class="label">Ngày sinh:</div>
                <div class="value">04/02/2006</div>
            </div>

            <div class="info-row">
                <div class="label">Email:</div>
                <div class="value">student@example.com</div>
            </div>

            <div class="info-row">
                <div class="label">Số điện thoại:</div>
                <div class="value">0123 456 789</div>
            </div>

            <div class="info-row">
                <div class="label">Chuyên ngành:</div>
                <div class="value">Công nghệ thông tin</div>
            </div>

            <div class="info-row">
                <div class="label">Trạng thái:</div>
                <div class="value">
                    <span class="status">Đang học</span>
                </div>
            </div>

        </div>
    </div>

</body>
