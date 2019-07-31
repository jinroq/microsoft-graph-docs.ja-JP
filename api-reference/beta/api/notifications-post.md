---
title: 通知を作成し送信する
description: 'Microsoft Graph を使用してユーザーを対象にした通知を作成し、送信します。 通知は Microsoft Graph 通知フィードストアに格納され、ユーザーがサインインしているすべてのデバイスエンドポイント上のすべてのアプリクライアントに送信されます。  '
localization_priority: Normal
ms.prod: project-rome
doc_type: apiPageType
author: ''
ms.openlocfilehash: a5ed743e93a5cafcb7ee919acbbcee5f2734a5de
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35992648"
---
# <a name="create-and-send-a-notification"></a><span data-ttu-id="9610f-104">通知を作成し送信する</span><span class="sxs-lookup"><span data-stu-id="9610f-104">Create and send a notification</span></span>
[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9610f-105">Microsoft Graph を使用してユーザーを対象にした通知を作成し、送信します。</span><span class="sxs-lookup"><span data-stu-id="9610f-105">Create and send a notification targeting a user through Microsoft Graph.</span></span> <span data-ttu-id="9610f-106">通知は Microsoft Graph 通知フィードストアに格納され、ユーザーがサインインしているすべてのデバイスエンドポイント上のすべてのアプリクライアントに送信されます。</span><span class="sxs-lookup"><span data-stu-id="9610f-106">The notification is stored in the Microsoft Graph notification feed store, and is sent to all app clients on all device endpoints that the user is signed in to.</span></span>  
## <a name="permissions"></a><span data-ttu-id="9610f-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9610f-107">Permissions</span></span>
<span data-ttu-id="9610f-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9610f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9610f-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9610f-110">Permission type</span></span>      | <span data-ttu-id="9610f-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9610f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9610f-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9610f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9610f-113">Notifications.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="9610f-113">Notifications.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="9610f-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9610f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9610f-115">Notifications.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="9610f-115">Notifications.ReadWrite.CreatedByApp</span></span>    |

## <a name="http-request"></a><span data-ttu-id="9610f-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9610f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/notifications/
```
## <a name="request-headers"></a><span data-ttu-id="9610f-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9610f-117">Request headers</span></span>
|<span data-ttu-id="9610f-118">名前</span><span class="sxs-lookup"><span data-stu-id="9610f-118">Name</span></span> | <span data-ttu-id="9610f-119">型</span><span class="sxs-lookup"><span data-stu-id="9610f-119">Type</span></span> | <span data-ttu-id="9610f-120">説明</span><span class="sxs-lookup"><span data-stu-id="9610f-120">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="9610f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9610f-121">Authorization</span></span> | <span data-ttu-id="9610f-122">string</span><span class="sxs-lookup"><span data-stu-id="9610f-122">string</span></span> |<span data-ttu-id="9610f-123">認証ヘッダーは、呼び出し元の資格情報を渡すために使用されます。</span><span class="sxs-lookup"><span data-stu-id="9610f-123">The authorization header is used to pass the credentials of the calling party.</span></span> <span data-ttu-id="9610f-124">ベアラー {token}。</span><span class="sxs-lookup"><span data-stu-id="9610f-124">Bearer {token}.</span></span> <span data-ttu-id="9610f-125">必須です。</span><span class="sxs-lookup"><span data-stu-id="9610f-125">Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="9610f-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="9610f-126">Request body</span></span>
<span data-ttu-id="9610f-127">要求本文で、[通知](../resources/projectrome-notification.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="9610f-127">In the request body, supply a JSON representation of a [notification](../resources/projectrome-notification.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="9610f-128">応答</span><span class="sxs-lookup"><span data-stu-id="9610f-128">Response</span></span>
<span data-ttu-id="9610f-129">成功した場合、このメソッド`201 Created`は通知が正常に作成され、保存されたことを示す応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="9610f-129">If successful, this method returns the `201 Created` response code that indicates that the notification was successfully created and stored.</span></span> 
## <a name="example"></a><span data-ttu-id="9610f-130">例</span><span class="sxs-lookup"><span data-stu-id="9610f-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="9610f-131">要求</span><span class="sxs-lookup"><span data-stu-id="9610f-131">Request</span></span>
<span data-ttu-id="9610f-132">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9610f-132">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="9610f-133">応答</span><span class="sxs-lookup"><span data-stu-id="9610f-133">Response</span></span>
<span data-ttu-id="9610f-134">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9610f-134">The following is an example of the response.</span></span>

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


