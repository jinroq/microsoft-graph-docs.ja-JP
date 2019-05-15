---
title: 通知を作成し送信する
description: 'Microsoft Graph を使用してユーザーを対象にした通知を作成し、送信します。 通知は Microsoft Graph 通知フィードストアに格納され、ユーザーがサインインしているすべてのデバイスエンドポイント上のすべてのアプリクライアントに送信されます。  '
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 86e67d040dcae3a013d8848c638ffadca41e4f5f
ms.sourcegitcommit: 70ebcc469e2fdf2c31aeb6c5169f0101c3e698b0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/15/2019
ms.locfileid: "34063457"
---
# <a name="create-and-send-a-notification"></a><span data-ttu-id="950cd-104">通知を作成し送信する</span><span class="sxs-lookup"><span data-stu-id="950cd-104">Create and send a notification</span></span>
[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="950cd-105">Microsoft Graph を使用してユーザーを対象にした通知を作成し、送信します。</span><span class="sxs-lookup"><span data-stu-id="950cd-105">Create and send a notification targeting a user through Microsoft Graph.</span></span> <span data-ttu-id="950cd-106">通知は Microsoft Graph 通知フィードストアに格納され、ユーザーがサインインしているすべてのデバイスエンドポイント上のすべてのアプリクライアントに送信されます。</span><span class="sxs-lookup"><span data-stu-id="950cd-106">The notification is stored in the Microsoft Graph notification feed store, and is sent to all app clients on all device endpoints that the user is signed in to.</span></span>  
## <a name="permissions"></a><span data-ttu-id="950cd-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="950cd-107">Permissions</span></span>
<span data-ttu-id="950cd-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="950cd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="950cd-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="950cd-110">Permission type</span></span>      | <span data-ttu-id="950cd-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="950cd-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="950cd-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="950cd-112">Delegated (work or school account)</span></span> | <span data-ttu-id="950cd-113">Notifications.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="950cd-113">Notifications.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="950cd-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="950cd-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="950cd-115">Notifications.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="950cd-115">Notifications.ReadWrite.CreatedByApp</span></span>    |

## <a name="http-request"></a><span data-ttu-id="950cd-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="950cd-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/notifications/
```
## <a name="request-headers"></a><span data-ttu-id="950cd-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="950cd-117">Request headers</span></span>
|<span data-ttu-id="950cd-118">名前</span><span class="sxs-lookup"><span data-stu-id="950cd-118">Name</span></span> | <span data-ttu-id="950cd-119">種類</span><span class="sxs-lookup"><span data-stu-id="950cd-119">Type</span></span> | <span data-ttu-id="950cd-120">説明</span><span class="sxs-lookup"><span data-stu-id="950cd-120">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="950cd-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="950cd-121">Authorization</span></span> | <span data-ttu-id="950cd-122">string</span><span class="sxs-lookup"><span data-stu-id="950cd-122">string</span></span> |<span data-ttu-id="950cd-123">認証ヘッダーは、呼び出し元の資格情報を渡すために使用されます。</span><span class="sxs-lookup"><span data-stu-id="950cd-123">The authorization header is used to pass the credentials of the calling party.</span></span> <span data-ttu-id="950cd-124">ベアラー {token}。</span><span class="sxs-lookup"><span data-stu-id="950cd-124">Bearer {token}.</span></span> <span data-ttu-id="950cd-125">必須です。</span><span class="sxs-lookup"><span data-stu-id="950cd-125">Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="950cd-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="950cd-126">Request body</span></span>
<span data-ttu-id="950cd-127">要求本文で、[通知](../resources/projectrome-notification.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="950cd-127">In the request body, supply a JSON representation of a [notification](../resources/projectrome-notification.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="950cd-128">応答</span><span class="sxs-lookup"><span data-stu-id="950cd-128">Response</span></span>
<span data-ttu-id="950cd-129">成功した場合、このメソッド`201 Created`は通知が正常に作成され、保存されたことを示す応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="950cd-129">If successful, this method returns the `201 Created` response code that indicates that the notification was successfully created and stored.</span></span> 
## <a name="example"></a><span data-ttu-id="950cd-130">例</span><span class="sxs-lookup"><span data-stu-id="950cd-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="950cd-131">要求</span><span class="sxs-lookup"><span data-stu-id="950cd-131">Request</span></span>
<span data-ttu-id="950cd-132">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="950cd-132">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="950cd-133">応答</span><span class="sxs-lookup"><span data-stu-id="950cd-133">Response</span></span>
<span data-ttu-id="950cd-134">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="950cd-134">The following is an example of the response.</span></span>

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


