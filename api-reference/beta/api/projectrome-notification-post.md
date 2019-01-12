---
title: 作成し、通知を送信します。
description: '作成し、Microsoft Graph を使用してユーザーを対象とする通知を送信します。 通知は、フィード ストア、Microsoft Graph の通知に格納され、ユーザーがサインインしてデバイスのすべてのエンドポイント上のすべてのアプリケーション クライアントに送信されます。  '
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: d8258e0da04f199a0f40bdb2a2ec85e01d5d5faf
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27975933"
---
# <a name="create-and-send-a-notification"></a><span data-ttu-id="da48c-104">作成し、通知を送信します。</span><span class="sxs-lookup"><span data-stu-id="da48c-104">Create and send a notification</span></span>
> <span data-ttu-id="da48c-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="da48c-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="da48c-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="da48c-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="da48c-107">作成し、Microsoft Graph を使用してユーザーを対象とする通知を送信します。</span><span class="sxs-lookup"><span data-stu-id="da48c-107">Create and send a notification targeting a user through Microsoft Graph.</span></span> <span data-ttu-id="da48c-108">通知は、フィード ストア、Microsoft Graph の通知に格納され、ユーザーがサインインしてデバイスのすべてのエンドポイント上のすべてのアプリケーション クライアントに送信されます。</span><span class="sxs-lookup"><span data-stu-id="da48c-108">The notification is stored in the Microsoft Graph notification feed store, and is sent to all app clients on all device endpoints that the user is signed in to.</span></span>  
## <a name="permissions"></a><span data-ttu-id="da48c-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="da48c-109">Permissions</span></span>
<span data-ttu-id="da48c-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="da48c-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da48c-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="da48c-112">Permission type</span></span>      | <span data-ttu-id="da48c-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="da48c-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="da48c-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="da48c-114">Delegated (work or school account)</span></span> | <span data-ttu-id="da48c-115">Notifications.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="da48c-115">Notifications.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="da48c-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="da48c-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da48c-117">Notifications.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="da48c-117">Notifications.ReadWrite.CreatedByApp</span></span>    |

## <a name="http-request"></a><span data-ttu-id="da48c-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="da48c-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/notifications/
```
## <a name="request-headers"></a><span data-ttu-id="da48c-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="da48c-119">Request headers</span></span>
|<span data-ttu-id="da48c-120">名前</span><span class="sxs-lookup"><span data-stu-id="da48c-120">Name</span></span> | <span data-ttu-id="da48c-121">種類</span><span class="sxs-lookup"><span data-stu-id="da48c-121">Type</span></span> | <span data-ttu-id="da48c-122">説明</span><span class="sxs-lookup"><span data-stu-id="da48c-122">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="da48c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="da48c-123">Authorization</span></span> | <span data-ttu-id="da48c-124">string</span><span class="sxs-lookup"><span data-stu-id="da48c-124">string</span></span> |<span data-ttu-id="da48c-125">承認ヘッダーを使用して、呼び出し元の関係者の資格情報を渡します。</span><span class="sxs-lookup"><span data-stu-id="da48c-125">The authorization header is used to pass the credentials of the calling party.</span></span> <span data-ttu-id="da48c-126">ベアラー {トークンが記述されています。</span><span class="sxs-lookup"><span data-stu-id="da48c-126">Bearer {token}.</span></span> <span data-ttu-id="da48c-127">必須。</span><span class="sxs-lookup"><span data-stu-id="da48c-127">Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="da48c-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="da48c-128">Request body</span></span>
<span data-ttu-id="da48c-129">要求の本文には、[通知](../resources/projectrome-notification.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="da48c-129">In the request body, supply a JSON representation of a [notification](../resources/projectrome-notification.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="da48c-130">応答</span><span class="sxs-lookup"><span data-stu-id="da48c-130">Response</span></span>
<span data-ttu-id="da48c-131">かどうかは成功すると、このメソッドが返されます、 `201 Created` 、通知が正常に作成され保存されていることを示す応答コード。</span><span class="sxs-lookup"><span data-stu-id="da48c-131">If successful, this method returns the `201 Created` response code that indicates that the notification was successfully created and stored.</span></span> 
## <a name="example"></a><span data-ttu-id="da48c-132">例</span><span class="sxs-lookup"><span data-stu-id="da48c-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="da48c-133">要求</span><span class="sxs-lookup"><span data-stu-id="da48c-133">Request</span></span>
<span data-ttu-id="da48c-134">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="da48c-134">The following is an example of the request.</span></span>

```http
POST https://graph.microsoft.com/beta/me/notifications/
Content-type: application/json

{
    "targetHostName": "graphnotifications.sample.windows.com",
    "appNotificationId": "testDirectToastNotification",
    "expirationDateTime": "2018-08-29T23:51:33.000Z",
    "payload": {
        "visualContent": {
            "title": "Hello World!",
            "body": "Notifications are Great!"
        }
    },
    "targetPolicy": {
        "platformTypes": [
        "windows",
        "android"
        ]
    },
    "priority": "High",
    "groupName": "TestGroup",
    "displayTimeToLive": "23"
}
```

#### <a name="response"></a><span data-ttu-id="da48c-135">応答</span><span class="sxs-lookup"><span data-stu-id="da48c-135">Response</span></span>
<span data-ttu-id="da48c-136">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="da48c-136">The following is an example of the response.</span></span>

```http
HTTP/1.1 201
Content-Type: application/json
location: https://graph.microsoft.com/beta/me/notifications/518c4fb1-c565-4d67-95c4-bcc3eb8eda1b

{
    "@odata.context": "https://graph.microsoft.com/test872018/$metadata#users('graphNotificationsUser%40contoso.com')/notifications/$entity",
    "appNotificationId": "testDirectToastNotification",
    "displayTimeToLive": 23,
    "expirationDateTime": "2018-08-24T12:31:53.858Z",
    "groupName": "TestGroup",
    "id": "cd5c5e6a-99ce-470a-9982-c47635e73620",
    "priority": "1",
    "payload": {
        "visualContent": {
            "title": "Hello World!",
            "body": "Notifications are Great!"
        }
    }
}
```


