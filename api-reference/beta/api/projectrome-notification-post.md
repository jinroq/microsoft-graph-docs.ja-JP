---
title: 作成し、通知を送信します。
description: '作成し、Microsoft Graph を使用してユーザーを対象とする通知を送信します。 通知は、フィード ストア、Microsoft Graph の通知に格納され、ユーザーがサインインしてデバイスのすべてのエンドポイント上のすべてのアプリケーション クライアントに送信されます。  '
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 70c7992a6fd323b909d948976132304fa04393c4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528446"
---
# <a name="create-and-send-a-notification"></a><span data-ttu-id="d946c-104">作成し、通知を送信します。</span><span class="sxs-lookup"><span data-stu-id="d946c-104">Create and send a notification</span></span>
[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d946c-105">作成し、Microsoft Graph を使用してユーザーを対象とする通知を送信します。</span><span class="sxs-lookup"><span data-stu-id="d946c-105">Create and send a notification targeting a user through Microsoft Graph.</span></span> <span data-ttu-id="d946c-106">通知は、フィード ストア、Microsoft Graph の通知に格納され、ユーザーがサインインしてデバイスのすべてのエンドポイント上のすべてのアプリケーション クライアントに送信されます。</span><span class="sxs-lookup"><span data-stu-id="d946c-106">The notification is stored in the Microsoft Graph notification feed store, and is sent to all app clients on all device endpoints that the user is signed in to.</span></span>  
## <a name="permissions"></a><span data-ttu-id="d946c-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d946c-107">Permissions</span></span>
<span data-ttu-id="d946c-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d946c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d946c-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d946c-110">Permission type</span></span>      | <span data-ttu-id="d946c-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d946c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d946c-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d946c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d946c-113">Notifications.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="d946c-113">Notifications.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="d946c-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d946c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d946c-115">Notifications.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="d946c-115">Notifications.ReadWrite.CreatedByApp</span></span>    |

## <a name="http-request"></a><span data-ttu-id="d946c-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d946c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/notifications/
```
## <a name="request-headers"></a><span data-ttu-id="d946c-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d946c-117">Request headers</span></span>
|<span data-ttu-id="d946c-118">名前</span><span class="sxs-lookup"><span data-stu-id="d946c-118">Name</span></span> | <span data-ttu-id="d946c-119">型</span><span class="sxs-lookup"><span data-stu-id="d946c-119">Type</span></span> | <span data-ttu-id="d946c-120">説明</span><span class="sxs-lookup"><span data-stu-id="d946c-120">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="d946c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d946c-121">Authorization</span></span> | <span data-ttu-id="d946c-122">string</span><span class="sxs-lookup"><span data-stu-id="d946c-122">string</span></span> |<span data-ttu-id="d946c-123">承認ヘッダーを使用して、呼び出し元の関係者の資格情報を渡します。</span><span class="sxs-lookup"><span data-stu-id="d946c-123">The authorization header is used to pass the credentials of the calling party.</span></span> <span data-ttu-id="d946c-124">ベアラー トークン</span><span class="sxs-lookup"><span data-stu-id="d946c-124">Bearer {token}.</span></span> <span data-ttu-id="d946c-125">必須です。</span><span class="sxs-lookup"><span data-stu-id="d946c-125">Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="d946c-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="d946c-126">Request body</span></span>
<span data-ttu-id="d946c-127">要求の本文には、[通知](../resources/projectrome-notification.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="d946c-127">In the request body, supply a JSON representation of a [notification](../resources/projectrome-notification.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d946c-128">応答</span><span class="sxs-lookup"><span data-stu-id="d946c-128">Response</span></span>
<span data-ttu-id="d946c-129">かどうかは成功すると、このメソッドが返されます、 `201 Created` 、通知が正常に作成され保存されていることを示す応答コード。</span><span class="sxs-lookup"><span data-stu-id="d946c-129">If successful, this method returns the `201 Created` response code that indicates that the notification was successfully created and stored.</span></span> 
## <a name="example"></a><span data-ttu-id="d946c-130">例</span><span class="sxs-lookup"><span data-stu-id="d946c-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="d946c-131">要求</span><span class="sxs-lookup"><span data-stu-id="d946c-131">Request</span></span>
<span data-ttu-id="d946c-132">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d946c-132">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="d946c-133">応答</span><span class="sxs-lookup"><span data-stu-id="d946c-133">Response</span></span>
<span data-ttu-id="d946c-134">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d946c-134">The following is an example of the response.</span></span>

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


<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/projectrome-notification-post.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
