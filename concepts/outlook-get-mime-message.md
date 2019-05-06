---
title: メッセージの MIME コンテンツを取得する
description: Multipurpose Internet Mail Extensions (MIME) は業界メール標準です。 `$value` セグメントを使用して Outlook メッセージの MIME コンテンツを取得できるようになりました。
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: a0b71e3e87a845c995ec2792bab12fc0fc446b59
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32655805"
---
# <a name="get-mime-content-of-a-message-preview"></a><span data-ttu-id="78734-104">メッセージの MIME コンテンツを取得する (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="78734-104">Get MIME content of a message (preview)</span></span>

<span data-ttu-id="78734-105">MIME は業界メール標準です。</span><span class="sxs-lookup"><span data-stu-id="78734-105">MIME is an industry email standard.</span></span> <span data-ttu-id="78734-106">多くのメール アプリケーションは、MIME 形式でメッセージを作成し、.EML という拡張子のファイルにそのメッセージを保存します。</span><span class="sxs-lookup"><span data-stu-id="78734-106">Many email applications create messages in MIME format and save them in files with the .EML extension.</span></span> 

<span data-ttu-id="78734-107">Outlook は MIME 形式でメッセージを_保存しません_が、Outlook メッセージの本文を MIME 形式で取得できる方法が 2 つあります。</span><span class="sxs-lookup"><span data-stu-id="78734-107">Even though Outlook _does not save_ messages in MIME format, there are two ways you can get an Outlook message body in MIME format:</span></span>

- <span data-ttu-id="78734-108">そのメッセージの get-message 操作に `$value` セグメントを追加できます。</span><span class="sxs-lookup"><span data-stu-id="78734-108">You can append a `$value` segment to a get-message operation on that message.</span></span>
- <span data-ttu-id="78734-109">そのメッセージが Outlook アイテムやグループ投稿に添付されている場合、そのアイテムまたはグループ投稿の get-attachment 操作に `$value` セグメントを追加できます。</span><span class="sxs-lookup"><span data-stu-id="78734-109">If the message is attached to an Outlook item or group post, you can append a `$value` segment to a get-attachment operation on that item or group post.</span></span>

<span data-ttu-id="78734-110">どちらの場合も、get-message 操作や get-attachment 操作を適用するため、Outlook アイテムやグループ投稿に[アクセスするための適切なアクセス許可](permissions-reference.md#mail-permissions)がアプリに必要です。</span><span class="sxs-lookup"><span data-stu-id="78734-110">In either case, your app must have the appropriate [permissions to access](permissions-reference.md#mail-permissions) the Outlook item or group post in order to apply the get-message or get-attachment operation.</span></span> 

<span data-ttu-id="78734-111">その後、メッセージ本文のコンテンツを .EML ファイルに保存し、CRM、ERP、バグ追跡などに使用するビジネス システムのレコードにそのファイルを添付できます。</span><span class="sxs-lookup"><span data-stu-id="78734-111">You can then save the message body content in a .EML file and attach the file to records in business systems, such as those for CRM, ERP, and bug tracking.</span></span> 

> <span data-ttu-id="78734-112">**重要:** MIME メッセージを取得する機能は、現在、/beta バージョンでのみ利用できます。</span><span class="sxs-lookup"><span data-stu-id="78734-112">**Important:** The capability to get MIME message body is currently available only in the /beta version.</span></span> <span data-ttu-id="78734-113">プレビュー段階の他の API と同様、変更される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="78734-113">Similar to other APIs in preview status, it is subject to change.</span></span> <span data-ttu-id="78734-114">運用アプリでは、この機能を使用しないでください。</span><span class="sxs-lookup"><span data-stu-id="78734-114">Do not use this capability in production apps.</span></span> <span data-ttu-id="78734-115">詳細については、「[バージョン管理とサポート](versioning-and-support.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="78734-115">For more information about API versions, see [Versioning and support](versioning-and-support.md).</span></span>

## <a name="what-is-mime"></a><span data-ttu-id="78734-116">MIME とは</span><span class="sxs-lookup"><span data-stu-id="78734-116">What is MIME?</span></span>

<span data-ttu-id="78734-117">MIME は、次の種類のコンテンツを SMTP 経由で送信するためにインターネット メールで使用される標準です。</span><span class="sxs-lookup"><span data-stu-id="78734-117">MIME is a standard used by internet email to transmit the following types of content via SMTP:</span></span> 

- <span data-ttu-id="78734-118">プレーンテキスト メッセージ</span><span class="sxs-lookup"><span data-stu-id="78734-118">plain text message</span></span>
- <span data-ttu-id="78734-119">代替コンテンツを含むメッセージ (プレーンテキストと HTML 両方など)</span><span class="sxs-lookup"><span data-stu-id="78734-119">Message with alternative content (i.e., in both plain text and HTML)</span></span>
- <span data-ttu-id="78734-120">元のメッセージが添付された返信メッセージ</span><span class="sxs-lookup"><span data-stu-id="78734-120">Reply message with the original message attached</span></span>
- <span data-ttu-id="78734-121">画像、オーディオ、ビデオ、アプリケーション ファイルが添付されたテキスト メッセージ</span><span class="sxs-lookup"><span data-stu-id="78734-121">Text message with attachments of image, audio, video, or application files</span></span>  
- <span data-ttu-id="78734-122">他のメッセージ コンストラクト</span><span class="sxs-lookup"><span data-stu-id="78734-122">Other message constructs</span></span>

<span data-ttu-id="78734-123">メッセージに含まれる一般的な MIME ヘッダーを次に示します。</span><span class="sxs-lookup"><span data-stu-id="78734-123">The following are typical MIME headers in a message.</span></span> <span data-ttu-id="78734-124">詳細については、「[RFC 2045](https://tools.ietf.org/html/rfc2045)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="78734-124">For more information, see [RFC 2045](https://tools.ietf.org/html/rfc2045).</span></span>

- <span data-ttu-id="78734-125">`MIME-Version` - メッセージが MIME 形式であることを示します。</span><span class="sxs-lookup"><span data-stu-id="78734-125">`MIME-Version` - Indicates the message is MIME-formatted.</span></span>
- <span data-ttu-id="78734-126">`Content-Type` - メッセージまたはメッセージの一部のメディア タイプを、*type* および *subtype* によって示します。</span><span class="sxs-lookup"><span data-stu-id="78734-126">`Content-Type` - Indicates the media type of the message or a part of the message, represented by a *type* and *subtype*.</span></span> <span data-ttu-id="78734-127">これには、`boundary` フィールドも含まれます。このフィールドは、`Content-Type` の位置に応じ、文字列を MIME の境界またはカプセル化の境界として指定します。</span><span class="sxs-lookup"><span data-stu-id="78734-127">It also includes a `boundary` field which specifies a string as the MIME boundary or as the encapsulation boundary, depending on the location of `Content-Type`.</span></span> 
- <span data-ttu-id="78734-128">`Content-Disposition` - 添付ファイルの提示スタイル (`inline` または `attachment`)、ファイル名、作成日と最終変更日など、添付ファイルに関する詳細を提供します。</span><span class="sxs-lookup"><span data-stu-id="78734-128">`Content-Disposition` - Provides details of an attachment such as its presentation style (`inline` or `attachment`), filenames, and creation and last modification dates.</span></span>
- <span data-ttu-id="78734-129">`Content-Transfer-Encoding` - バイナリ データを表すエンコード方法を指定します。</span><span class="sxs-lookup"><span data-stu-id="78734-129">`Content-Transfer-Encoding` - Specifies the encoding method to represent binary data.</span></span>

## <a name="get-mime-content-of-an-outlook-message"></a><span data-ttu-id="78734-130">Outlook メッセージの MIME コンテンツを取得する</span><span class="sxs-lookup"><span data-stu-id="78734-130">Get MIME content of an Outlook message</span></span>

<span data-ttu-id="78734-131">[メッセージを取得](/graph/api/message-get?view=graph-rest-beta)する際に `$value` セグメントを追加することにより、メッセージを MIME 形式で取得できます。</span><span class="sxs-lookup"><span data-stu-id="78734-131">You can get the MIME representation of a message by appending the `$value` segment when [getting the message](/graph/api/message-get?view=graph-rest-beta):</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /users/{id}/messages/{id}/$value
```

### <a name="example"></a><span data-ttu-id="78734-132">例</span><span class="sxs-lookup"><span data-stu-id="78734-132">Example</span></span>

<span data-ttu-id="78734-133">次の例では、サインイン ユーザーのメールボックスに含まれるメッセージを、その MIME コンテンツを含めて返すように要求しています。</span><span class="sxs-lookup"><span data-stu-id="78734-133">The following is an example that requests a message in the signed-in user's mailbox to be returned with its MIME content.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/4aade2547798441eab5188a7a2436bc1/$value
```

<span data-ttu-id="78734-134">応答は次のようになります。</span><span class="sxs-lookup"><span data-stu-id="78734-134">The following is the XML response.</span></span> <span data-ttu-id="78734-135">MIME コンテンツは `MIME-Version` ヘッダーから始まります。</span><span class="sxs-lookup"><span data-stu-id="78734-135">The MIME content begins with the `MIME-Version` header.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
Received: from contoso.com (10.194.241.197) by 
contoso.com (10.194.241.197) with Microsoft 
SMTP Server (version=TLS1_2, 
cipher=TLS_ECDHE_RSA_WITH_AES_256_CBC_SHA384_P256) id 15.1.1374.0 via Mailbox 
Transport; Mon, 4 Sep 2017 03:00:08 -0700 
Received: from contoso.com (10.194.241.197) by 
contoso.com (10.194.241.197) with Microsoft 
SMTP Server (version=TLS1_2, 
cipher=TLS_ECDHE_RSA_WITH_AES_256_CBC_SHA384_P256) id 15.1.1374.0; Mon, 4 Sep 
2017 03:00:07 -0700 
Received: from contoso.com 
(fe80::5bf:5059:4ca0:5017) by contoso.com 
(fe80::5bf:5059:4ca0:5017%12) with mapi id 15.01.1374.000; Mon, 4 Sep 2017 
03:00:01 -0700 
From: Administrator <admin@contoso.com> 
To: Administrator <admin@contoso.com> 
Subject: This email has attachment. 
Thread-Topic: This email has attachment. 
Thread-Index: AQHTJWSHSywMzSz8o0OJud48nG50GQ== 
Date: Mon, 4 Sep 2017 10:00:00 +0000 
Message-ID: 
                <4aade2547798441eab5188a7a2436bc1@contoso.com> 
Accept-Language: en-US 
Content-Language: en-US 
X-MS-Exchange-Organization-AuthAs: Internal 
X-MS-Exchange-Organization-AuthMechanism: 04 
X-MS-Exchange-Organization-AuthSource: 
                contoso.com 
X-MS-Has-Attach: yes 
X-MS-Exchange-Organization-Network-Message-Id: 
                0ffdb402-ec03-42c8-5d32-08d4f37bb517 
X-MS-Exchange-Organization-SCL: -1 
X-MS-TNEF-Correlator: 
X-MS-Exchange-Organization-RecordReviewCfmType: 0 
x-ms-publictraffictype: Emai

```http
MIME-Version: 1.0 
Content-Type: multipart/mixed; 
                boundary="_004_4aade2547798441eab5188a7a2436bc1contoso_" 
 
--_004_4aade2547798441eab5188a7a2436bc1contoso_ 
Content-Type: multipart/alternative; 
                boundary="_000_4aade2547798441eab5188a7a2436bc1contoso_" 
 
--_000_4aade2547798441eab5188a7a2436bc1contoso_ 
Content-Type: text/plain; charset="iso-8859-1" 
Content-Transfer-Encoding: quoted-printable 
 
The attachment is an email. 
 
--_000_4aade2547798441eab5188a7a2436bc1contoso_ 
Content-Type: text/html; charset="iso-8859-1" 
Content-Transfer-Encoding: quoted-printable 
 
<html> 
<head> 
<meta http-equiv=3D"Content-Type" content=3D"text/html; charset=3Diso-8859-= 
1"> 
<style type=3D"text/css" style=3D"display:none;"><!-- P {margin-top:0;margi= 
n-bottom:0;} --></style> 
</head> 
<body dir=3D"ltr"> 
<div id=3D"divtagdefaultwrapper" style=3D"font-size:12pt;color:#000000;font= 
-family:Calibri,Helvetica,sans-serif;" dir=3D"ltr"> 
<p>The attachment is an email.</p> 
</div> 
</body> 
</html> 
 
--_000_4aade2547798441eab5188a7a2436bc1contoso_-- 
 
--_004_4aade2547798441eab5188a7a2436bc1contoso_ 
Content-Type: application/octet-stream; name="Attachment email.eml" 
Content-Description: Attachment email.eml 
Content-Disposition: attachment; filename="Attachment email.eml"; size=408; 
                creation-date="Mon, 04 Sep 2017 09:59:43 GMT"; 
                modification-date="Mon, 04 Sep 2017 09:59:43 GMT" 
Content-Transfer-Encoding: base64 
 
RnJvbToJQWRtaW5pc3RyYXRvciA8YWRtaW5AdGVuYW50LUVYSEItMTQ3MS5jb20+DQpTZW50OglN 
b25kYXksIFNlcHRlbWJlciA0LCAyMDE3IDM6MjYgUE0NClRvOglTcml2YXJkaGFuIEhlYmJhcg0K 
U3ViamVjdDoJQXR0YWNobWVudCBlbWFpbA0KDQpJIHdpbGwgYXR0YWNoIHRoaXMgZW1haWwgdG8g 
YW5vdGhlciBtYWlsLg0K 
 
--_004_4aade2547798441eab5188a7a2436bc1contoso_-- 
```

## <a name="get-mime-content-of-an-outlook-message-attached-to-an-outlook-item-or-group-post"></a><span data-ttu-id="78734-136">Outlook アイテムまたはグループ投稿に添付された Outlook メッセージの MIME コンテンツを取得する</span><span class="sxs-lookup"><span data-stu-id="78734-136">Get MIME content of an Outlook message attached to an Outlook item or group post</span></span>

<span data-ttu-id="78734-137">ユーザーのアプリがアクセスできる Outlook の[イベント](/graph/api/resources/event?view=graph-rest-beta)、[メッセージ](/graph/api/resources/message?view=graph-rest-beta)、[タスク](/graph/api/resources/outlooktask?view=graph-rest-beta)、グループ[投稿](/graph/api/resources/post?view=graph-rest-beta)に Outlook メッセージが添付されている場合、その Outlook メッセージも MIME 形式で取得できます。</span><span class="sxs-lookup"><span data-stu-id="78734-137">You can also get the MIME representation of an Outlook message, if the message has been attached to an Outlook [event](/graph/api/resources/event?view=graph-rest-beta), [message](/graph/api/resources/message?view=graph-rest-beta), [task](/graph/api/resources/outlooktask?view=graph-rest-beta), or group [post](/graph/api/resources/post?view=graph-rest-beta) that your app can access.</span></span>

<span data-ttu-id="78734-138">これには、メッセージの添付ファイルを特定し、[その添付ファイルを取得](/graph/api/attachment-get?view=graph-rest-beta#get-the-raw-contents-of-a-file-or-item-attachment
)する際に `$value` セグメントを追加します。</span><span class="sxs-lookup"><span data-stu-id="78734-138">To do that, identify the message attachment, and append the `$value` segment when [getting that attachment](/graph/api/attachment-get?view=graph-rest-beta#get-the-raw-contents-of-a-file-or-item-attachment
).</span></span> <span data-ttu-id="78734-139">次に、添付ファイルにアクセスする一般的な方法をいくつか示します。</span><span class="sxs-lookup"><span data-stu-id="78734-139">The following shows a few common ways to access an attachment.</span></span> <span data-ttu-id="78734-140">詳細については、「[添付ファイルを取得する](/graph/api/attachment-get?view=graph-rest-beta#http-request)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="78734-140">See [get attachment](/graph/api/attachment-get?view=graph-rest-beta#http-request) for more information.</span></span>

<span data-ttu-id="78734-141">メッセージがユーザーの既定のカレンダーのイベントに添付されている場合:</span><span class="sxs-lookup"><span data-stu-id="78734-141">If the message is attached to an event in the user's default calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id}/events/{id}/attachments/{id}/$value
```

<span data-ttu-id="78734-142">メッセージがユーザーのメールボックスの別のメッセージに添付されている場合:</span><span class="sxs-lookup"><span data-stu-id="78734-142">If the message is attached to another message in the user's mailbox:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id}/messages/{id}/attachments/{id}/$value
```

<span data-ttu-id="78734-143">メッセージがユーザーの既定のタスク フォルダーの Outlook タスクに添付されている場合:</span><span class="sxs-lookup"><span data-stu-id="78734-143">If the message is attached to an Outlook task in the user's default task folder:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id}/outlook/tasks/{id}/attachments/{id}/$value
```

<span data-ttu-id="78734-144">メッセージが指定されたグループ投稿に添付されている場合:</span><span class="sxs-lookup"><span data-stu-id="78734-144">If the message is attached to the specified group post:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments/{id}/$value
```

### <a name="example"></a><span data-ttu-id="78734-145">例</span><span class="sxs-lookup"><span data-stu-id="78734-145">Example</span></span>

<span data-ttu-id="78734-146">次の例では、別のメッセージに添付されていたメッセージを取得し、その本文を MIME 形式で返しています。</span><span class="sxs-lookup"><span data-stu-id="78734-146">The following is an example that gets a message that has been attached to another message, and returns the body in MIME format.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/messages/AAMkAGUAAA7XW-lAAA=/attachments/AAMkAGUAAA7XW-lAAABEgAQAFBZJBq4EN5FlCSvNV-M-FI=/$value
```

<span data-ttu-id="78734-147">応答は次のようになります。</span><span class="sxs-lookup"><span data-stu-id="78734-147">The following is the XML response.</span></span> <span data-ttu-id="78734-148">MIME コンテンツは `MIME-Version` ヘッダーから始まります。</span><span class="sxs-lookup"><span data-stu-id="78734-148">The MIME content begins with the `MIME-Version` header.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
Received: from MWHPR22MB0302.namprd22.prod.outlook.com (2603:10b6:104:5::23)
 by MWHPR2201MB1053.namprd22.prod.outlook.com with HTTPS via
 CO2PR04CA0193.NAMPRD04.PROD.OUTLOOK.COM; Mon, 22 Apr 2019 19:48:20 +0000
Received: from MWHPR22MB1007.namprd22.prod.outlook.com (10.172.167.21) by
 MWHPR22MB0302.namprd22.prod.outlook.com (10.173.53.146) with Microsoft SMTP
 Server (version=TLS1_2, cipher=TLS_ECDHE_RSA_WITH_AES_256_GCM_SHA384) id
 15.20.1813.12; Mon, 22 Apr 2019 19:48:16 +0000
Received: from MWHPR22MB1007.namprd22.prod.outlook.com
 ([fe80::1d05:c2d3:92a:f8dc]) by MWHPR22MB1007.namprd22.prod.outlook.com
 ([fe80::1d05:c2d3:92a:f8dc%9]) with mapi id 15.20.1813.017; Mon, 22 Apr 2019
 19:48:16 +0000
From: Adele Vance <AdeleV@contoso.OnMicrosoft.com>
To: Megan Bowen <MeganB@contoso.OnMicrosoft.com>
Subject: Press conference
Thread-Topic: Press conference
Thread-Index: AQHU+UQNzFWFTilRjECtpiWorLYxqA==
Date: Mon, 22 Apr 2019 19:48:16 +0000
Message-ID:
    <MWHPR22MB100769D1513B3DC0F007B2ECD4220@MWHPR22MB1007.namprd22.prod.outlook.com>
Accept-Language: en-US
Content-Language: en-US
X-MS-Exchange-Organization-AuthAs: Internal
X-MS-Exchange-Organization-AuthMechanism: 04
X-MS-Exchange-Organization-AuthSource: MWHPR22MB1007.namprd22.prod.outlook.com
X-MS-Has-Attach:
X-MS-Exchange-Organization-Network-Message-Id:
    88bed46b-a860-40fb-591e-08d6c75b76c1
X-MS-Exchange-Organization-SCL: -1
X-MS-TNEF-Correlator:
X-MS-Exchange-Organization-RecordReviewCfmType: 0
x-ms-publictraffictype: Email
authentication-results: contoso.OnMicrosoft.com; dkim=none (message not
 signed) header.d=none;contoso.OnMicrosoft.com; dmarc=none action=none
 header.from=contoso.OnMicrosoft.com;
x-originating-ip: [2001:4898:80e8:9:9607:7cf8:4576:961c]
x-ms-office365-filtering-correlation-id: 88bed46b-a860-40fb-591e-08d6c75b76c1
x-microsoft-antispam:
    BCL:0;PCL:0;RULEID:(2390118)(7020095)(4652040)(7021145)(8989299)(4534185)(7022145)(4603075)(4627221)(201702281549075)(8990200)(5600141)(711020)(4605104)(2017052603328)(7177060)(7171020)(7173020)(7193020);SRVR:MWHPR22MB0302;
x-ms-traffictypediagnostic: MWHPR22MB0302:
X-Microsoft-Antispam-Mailbox-Delivery:
    ucf:0;jmr:0;ex:0;auth:0;dest:I;ENG:(750119)(520011016)(706158)(944506303)(944626516);
X-Microsoft-Antispam-Message-Info:
    twccJ5SmB7ZvueSjaTBdmtD3489zlRiHPqiO3DBEil1jBx5xhl/5G/fK2GLgdH0klkE2uoUAAvdvpmxiJezwxCtmn11Nq3kvaOuypDL2TDVdYvWkTfSt4SYfVTp34iBoDlvOEbTh8LTl5J/dz98cgvoRdiE7TUJBXTGvUyVTQX1LG7Xg1hNXMu6XLng6Axdn/ka2NUhmzOa3hEl9yoUI8g3G66Vq3zzVRQFpS+P5+/d1LcbKHsuYMgZNBzBeM6dLnMnwOH9rKXqjV+d72YDnQw4SkbULkoEsQs2Vq0e4URDtkzQwHqcoPv1W2HE4pypmiqkl4M6lJtBccF3MWPP/xNxl6NL5gLSpZCILbg8gQ1UxxX8Kdhd4KWbDa3ayHLHBr11hMNFbGftcUZbZ6jrAtiIGYtGzaAxHqlYC3lUHXZIMdygT76enIJJwklQ1VIp4
Content-Type: multipart/alternative;
    boundary="_000_MWHPR22MB100769D1513B3DC0F007B2ECD4220MWHPR22MB1007namp_"
MIME-Version: 1.0

--_000_MWHPR22MB100769D1513B3DC0F007B2ECD4220MWHPR22MB1007namp_
Content-Type: text/plain; charset="iso-8859-1"
Content-Transfer-Encoding: quoted-printable

The press conference will be on May 15. We arranged to have the press gathe=
r at 2pm outside the main entrance.

--_000_MWHPR22MB100769D1513B3DC0F007B2ECD4220MWHPR22MB1007namp_
Content-Type: text/html; charset="iso-8859-1"
Content-Transfer-Encoding: quoted-printable

<html>
<head>
<meta http-equiv=3D"Content-Type" content=3D"text/html; charset=3Diso-8859-=
1">
<style type=3D"text/css" style=3D"display:none;"><!-- P {margin-top:0;margi=
n-bottom:0;} --></style>
</head>
<body dir=3D"ltr">
<div id=3D"divtagdefaultwrapper" style=3D"font-size:12pt;color:#000000;font=
-family:Calibri,Helvetica,sans-serif;" dir=3D"ltr">
<p style=3D"margin-top:0;margin-bottom:0">The press conference will be on M=
ay 15. We arranged to have the press gather at 2pm outside the main entranc=
e.</p>
</div>
</body>
</html>

--_000_MWHPR22MB100769D1513B3DC0F007B2ECD4220MWHPR22MB1007namp_--
```

## <a name="next-steps"></a><span data-ttu-id="78734-149">次の手順</span><span class="sxs-lookup"><span data-stu-id="78734-149">Next steps</span></span>

<span data-ttu-id="78734-150">詳細情報:</span><span class="sxs-lookup"><span data-stu-id="78734-150">Find out more about:</span></span>

- <span data-ttu-id="78734-151">イベント、メッセージ、Outlook タスク、グループ投稿に対する[アイテム添付ファイルの MIME コンテンツを取得する](/graph/api/attachment-get?view=graph-rest-beta#get-the-raw-contents-of-a-file-or-item-attachment)</span><span class="sxs-lookup"><span data-stu-id="78734-151">[Get the MIME content of an item attachment](/graph/api/attachment-get?view=graph-rest-beta#get-the-raw-contents-of-a-file-or-item-attachment) to an event, message, Outlook task, or group post</span></span>
- [<span data-ttu-id="78734-152">Outlook メールと統合する理由</span><span class="sxs-lookup"><span data-stu-id="78734-152">Why integrate with Outlook mail</span></span>](outlook-mail-concept-overview.md)
- <span data-ttu-id="78734-153">Microsoft Graph (ベータ版) の[メール API](/graph/api/resources/mail-api-overview?view=graph-rest-1.0) とその[用途](/graph/api/resources/mail-api-overview?view=graph-rest-beta#common-use-cases)。</span><span class="sxs-lookup"><span data-stu-id="78734-153">[Using the mail API](/graph/api/resources/mail-api-overview?view=graph-rest-1.0) and its [use cases](/graph/api/resources/mail-api-overview?view=graph-rest-beta#common-use-cases) in Microsoft Graph v1.0.</span></span>
