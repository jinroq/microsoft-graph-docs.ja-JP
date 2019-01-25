---
title: デバイス コマンドのステータスを取得します。
description: デバイス上には、コマンドのステータスを取得します。 ステータス コードの完全なリスト、actionStatus のリストを参照してください。
localization_priority: Normal
ms.openlocfilehash: ae5fe1f2b6b48c0a739911bd20370562e8540f18
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510114"
---
# <a name="get-device-command-status"></a><span data-ttu-id="ed987-104">デバイス コマンドのステータスを取得します。</span><span class="sxs-lookup"><span data-stu-id="ed987-104">Get device command status</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed987-105">デバイス上には、コマンドのステータスを取得します。</span><span class="sxs-lookup"><span data-stu-id="ed987-105">Get the status of a command on a device.</span></span> <span data-ttu-id="ed987-106">ステータス コードの完全なリスト、 [actionStatus のリスト](#list-of-actionstatus)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ed987-106">For the  full list of status codes, see [List of actionStatus](#list-of-actionstatus).</span></span>

## <a name="permissions"></a><span data-ttu-id="ed987-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ed987-107">Permissions</span></span>

<span data-ttu-id="ed987-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ed987-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed987-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ed987-110">Permission type</span></span>      | <span data-ttu-id="ed987-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ed987-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ed987-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ed987-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ed987-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ed987-113">Not supported.</span></span>    |
|<span data-ttu-id="ed987-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ed987-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed987-115">Device.Command</span><span class="sxs-lookup"><span data-stu-id="ed987-115">Device.Command</span></span>    |
|<span data-ttu-id="ed987-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ed987-116">Application</span></span> | <span data-ttu-id="ed987-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ed987-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ed987-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ed987-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices/{id}/commands/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ed987-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ed987-119">Request headers</span></span>

| <span data-ttu-id="ed987-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ed987-120">Header</span></span> |<span data-ttu-id="ed987-121">値</span><span class="sxs-lookup"><span data-stu-id="ed987-121">Value</span></span>
|:----|:------|
|<span data-ttu-id="ed987-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed987-122">Authorization</span></span>| <span data-ttu-id="ed987-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ed987-p104">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="ed987-125">承諾</span><span class="sxs-lookup"><span data-stu-id="ed987-125">Accept</span></span> | <span data-ttu-id="ed987-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ed987-126">application/json</span></span> |

## <a name="response"></a><span data-ttu-id="ed987-127">応答</span><span class="sxs-lookup"><span data-stu-id="ed987-127">Response</span></span>
<!-- { "blockType": "ignored" } -->

```http
HTTP/1.1 200 OK
```
<!-- { "blockType": "ignored" } -->

```json
  {
    "id": "0",
    "status": "requesting",
    "type": "null",
    "appServiceName": "null",
    "packageFamilyName": "null",
    "error": "null",
    "responsepayload": "null",
    "payload": "null",
    "permissionTicket": "null",
    "postBackUri": "null"
  }
```

## <a name="list-of-actionstatus"></a><span data-ttu-id="ed987-128">ActionStatus の一覧</span><span class="sxs-lookup"><span data-stu-id="ed987-128">List of actionStatus</span></span>

- <span data-ttu-id="ed987-129">要求、またはコマンドで作成された、処理を待機しています。</span><span class="sxs-lookup"><span data-stu-id="ed987-129">requesting, // Command has been created and is waiting to be processed</span></span>
- <span data-ttu-id="ed987-130">sentToTarget、またはターゲット ・ デバイスに送信されたコマンド/</span><span class="sxs-lookup"><span data-stu-id="ed987-130">sentToTarget, // Command has been sent to the target device</span></span>
- <span data-ttu-id="ed987-131">実行するとターゲット ・ デバイスは、コマンドの受信を確認し、実行しています。</span><span class="sxs-lookup"><span data-stu-id="ed987-131">executing, // Target device acknowledged receipt of the command and is executing it</span></span>
- <span data-ttu-id="ed987-132">完了すると、コマンドの実行が完了しました</span><span class="sxs-lookup"><span data-stu-id="ed987-132">completed, // Command execution completed</span></span>
- <span data-ttu-id="ed987-133">failedToSend、またはターゲット ・ デバイスにコマンドを送信するサービスが失敗したと</span><span class="sxs-lookup"><span data-stu-id="ed987-133">failedToSend, // Service failed to send command to target device</span></span>
- <span data-ttu-id="ed987-134">executionFailed、または、コマンドの実行に失敗しました</span><span class="sxs-lookup"><span data-stu-id="ed987-134">executionFailed, // Command execution failed</span></span>
- <span data-ttu-id="ed987-135">commandDropped、またはデバイスは ConnectedStandby の状態にある場合に、コマンドがクライアントによって削除/</span><span class="sxs-lookup"><span data-stu-id="ed987-135">commandDropped, // Command dropped by client if device is in ConnectedStandby state</span></span>
- <span data-ttu-id="ed987-136">取り消すには、//コマンドのキャンセル</span><span class="sxs-lookup"><span data-stu-id="ed987-136">cancel, // Cancel the command</span></span>
- <span data-ttu-id="ed987-137">キャンセルする、またはコマンドをキャンセルすると</span><span class="sxs-lookup"><span data-stu-id="ed987-137">cancelling, // Cancelling the command</span></span>
- <span data-ttu-id="ed987-138">キャンセルするには、//、コマンドは取り消されました</span><span class="sxs-lookup"><span data-stu-id="ed987-138">canceled, // Command has been cancelled</span></span>
- <span data-ttu-id="ed987-139">再試行、またはサービスがターゲットにコマンドを送信する再試行/</span><span class="sxs-lookup"><span data-stu-id="ed987-139">retry, // Service is retrying to send command to target</span></span>
- <span data-ttu-id="ed987-140">有効期限が切れた、またはコマンドの処理の有効期限を超過すると</span><span class="sxs-lookup"><span data-stu-id="ed987-140">expired, // Command processing exceeded expiry time</span></span>
- <span data-ttu-id="ed987-141">エラー、または内部またはコマンドの処理中にエラー</span><span class="sxs-lookup"><span data-stu-id="ed987-141">error, // Internal error while processing the command</span></span>
- <span data-ttu-id="ed987-142">カスタム/カスタム/ステータス</span><span class="sxs-lookup"><span data-stu-id="ed987-142">custom // Custom status</span></span>

## <a name="example"></a><span data-ttu-id="ed987-143">例</span><span class="sxs-lookup"><span data-stu-id="ed987-143">Example</span></span>

<span data-ttu-id="ed987-144">この例では、デバイスの ID とデバイスに発行されたコマンドの ID を必要があります。</span><span class="sxs-lookup"><span data-stu-id="ed987-144">In this example, you will need the ID of the device and the ID of the command that has been issued to a device.</span></span> <span data-ttu-id="ed987-145">GET を発行するときに ID が返されるデバイスの呼び出しの`/me/devices`の投稿を行うときに ID が返されるコマンドを呼び出すと`/me/devices/{id}/command`。</span><span class="sxs-lookup"><span data-stu-id="ed987-145">The device ID is returned when issuing a GET call to `/me/devices`, and the command ID is returned when doing a POST call on `/me/devices/{id}/command`.</span></span>

#### <a name="request"></a><span data-ttu-id="ed987-146">要求</span><span class="sxs-lookup"><span data-stu-id="ed987-146">Request</span></span>

<span data-ttu-id="ed987-147">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="ed987-147">The following example shows the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_command"
} -->
```http
GET me/devices/{id}/commands/{id}
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="ed987-148">応答</span><span class="sxs-lookup"><span data-stu-id="ed987-148">Response</span></span>

<span data-ttu-id="ed987-149">次の例は応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="ed987-149">The following example shows the response.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.commandobject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK

{
  "value":
  {
    "id": "0158355AD4D680CC4E2994CC009EFFD7337D1335FCA6ED266…",
    "status": "completed",
    "type": null,
    "appServiceName": null,
    "packageFamilyName": null,
    "error": null,
    "permissionTicket": null,
    "postBackUri": null,
    "payload": null
  }
}
```


## <a name="get-command-payload"></a><span data-ttu-id="ed987-150">コマンドのペイロードを取得します。</span><span class="sxs-lookup"><span data-stu-id="ed987-150">Get command payload</span></span>

<span data-ttu-id="ed987-151">デバイス上の特定のアクションの応答の内容を取得します。</span><span class="sxs-lookup"><span data-stu-id="ed987-151">Get a response payload for a specific action on a device.</span></span> <span data-ttu-id="ed987-152">応答の内容は、データを再度実行するために、アプリケーション サービスを照会するときに使用されます。</span><span class="sxs-lookup"><span data-stu-id="ed987-152">The response payload is used when querying an app service to carry data back.</span></span>


### <a name="permissions"></a><span data-ttu-id="ed987-153">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ed987-153">Permissions</span></span>

<span data-ttu-id="ed987-p107">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ed987-p107">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed987-156">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ed987-156">Permission type</span></span>      | <span data-ttu-id="ed987-157">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ed987-157">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ed987-158">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ed987-158">Delegated (work or school account)</span></span> | <span data-ttu-id="ed987-159">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ed987-159">Not supported.</span></span>    |
|<span data-ttu-id="ed987-160">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ed987-160">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed987-161">Device.Command</span><span class="sxs-lookup"><span data-stu-id="ed987-161">Device.Command</span></span>    |
|<span data-ttu-id="ed987-162">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ed987-162">Application</span></span> | <span data-ttu-id="ed987-163">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ed987-163">Not supported.</span></span> |

### <a name="http-request"></a><span data-ttu-id="ed987-164">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ed987-164">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices/{id}/command/{id}/responsePayload
```

### <a name="request-headers"></a><span data-ttu-id="ed987-165">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ed987-165">Request headers</span></span>

| <span data-ttu-id="ed987-166">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ed987-166">Header</span></span> |<span data-ttu-id="ed987-167">値</span><span class="sxs-lookup"><span data-stu-id="ed987-167">Value</span></span>
|:----|:------|
|<span data-ttu-id="ed987-168">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed987-168">Authorization</span></span>| <span data-ttu-id="ed987-p108">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ed987-p108">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="ed987-171">承諾</span><span class="sxs-lookup"><span data-stu-id="ed987-171">Accept</span></span> | <span data-ttu-id="ed987-172">application/json</span><span class="sxs-lookup"><span data-stu-id="ed987-172">application/json</span></span> |

### <a name="response"></a><span data-ttu-id="ed987-173">応答</span><span class="sxs-lookup"><span data-stu-id="ed987-173">Response</span></span>
<!-- { "blockType": "ignored" } -->

```http
HTTP/1.1 200 OK
```
<!-- { "blockType": "ignored" } -->

```json
{
  "@odata.context": "https://graph.microsoft.com/devices/$metadata#microsoft.graph.PayloadResponse",
  "MsIgnoredParameter":0,
  "CreationDate":"date-time",
  "Type":"Ok"
}
```

### <a name="example"></a><span data-ttu-id="ed987-174">例</span><span class="sxs-lookup"><span data-stu-id="ed987-174">Example</span></span>

<span data-ttu-id="ed987-175">この例では、デバイスの ID とデバイスに発行されたコマンドの ID を必要があります。</span><span class="sxs-lookup"><span data-stu-id="ed987-175">In this example, you will need the ID of the device and the ID of the command that has been issued to a device.</span></span> <span data-ttu-id="ed987-176">に対して GET を発行するときに ID が返されるデバイスを呼び出す`/me/devices`の投稿を行うときに ID が返されるコマンドを呼び出すと`/me/devices/{id}/command`。</span><span class="sxs-lookup"><span data-stu-id="ed987-176">The device ID is returned when issuing a GET call on `/me/devices`, and the command ID is returned when doing a POST call on `/me/devices/{id}/command`.</span></span>

#### <a name="request"></a><span data-ttu-id="ed987-177">要求</span><span class="sxs-lookup"><span data-stu-id="ed987-177">Request</span></span>

<span data-ttu-id="ed987-178">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="ed987-178">The following example shows the request.</span></span>

<!-- { 
  "blockType": "ignored",
  "name": "get_command_payload"
} -->
```http
GET me/devices/{id}/commands/{id}
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="ed987-179">応答</span><span class="sxs-lookup"><span data-stu-id="ed987-179">Response</span></span>

<span data-ttu-id="ed987-180">次の例は応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="ed987-180">The following example shows the response.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.commandobject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK

{
  "@odata.context": "https://graph.microsoft.com/devices/$metadata#microsoft.graph.PayloadResponse",
  "MsIgnoredParameter":0,
  "CreationDate":"04/27/2017",
  "Type":"Ok"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/get-device-command-status.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
