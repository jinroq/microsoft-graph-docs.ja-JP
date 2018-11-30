---
title: デバイス コマンドのステータスを取得します。
description: デバイス上には、コマンドのステータスを取得します。 ステータス コードの完全なリスト、actionStatus のリストを参照してください。
ms.openlocfilehash: 1e51d3b4366e87d9802518a50fe348d3ba0f250d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066355"
---
# <a name="get-device-command-status"></a><span data-ttu-id="e3fc4-104">デバイス コマンドのステータスを取得します。</span><span class="sxs-lookup"><span data-stu-id="e3fc4-104">Get device command status</span></span>

> <span data-ttu-id="e3fc4-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e3fc4-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e3fc4-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e3fc4-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e3fc4-107">デバイス上には、コマンドのステータスを取得します。</span><span class="sxs-lookup"><span data-stu-id="e3fc4-107">Get the status of a command on a device.</span></span> <span data-ttu-id="e3fc4-108">ステータス コードの完全なリスト、 [actionStatus のリスト](#list-of-actionstatus)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e3fc4-108">For the  full list of status codes, see [List of actionStatus](#list-of-actionstatus).</span></span>

## <a name="permissions"></a><span data-ttu-id="e3fc4-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e3fc4-109">Permissions</span></span>

<span data-ttu-id="e3fc4-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e3fc4-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3fc4-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e3fc4-112">Permission type</span></span>      | <span data-ttu-id="e3fc4-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e3fc4-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e3fc4-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e3fc4-114">Delegated (work or school account)</span></span> | <span data-ttu-id="e3fc4-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e3fc4-115">Not supported.</span></span>    |
|<span data-ttu-id="e3fc4-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e3fc4-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3fc4-117">Device.Command</span><span class="sxs-lookup"><span data-stu-id="e3fc4-117">Device.Command</span></span>    |
|<span data-ttu-id="e3fc4-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e3fc4-118">Application</span></span> | <span data-ttu-id="e3fc4-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e3fc4-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e3fc4-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e3fc4-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices/{id}/commands/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e3fc4-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e3fc4-121">Request headers</span></span>

| <span data-ttu-id="e3fc4-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e3fc4-122">Header</span></span> |<span data-ttu-id="e3fc4-123">値</span><span class="sxs-lookup"><span data-stu-id="e3fc4-123">Value</span></span>
|:----|:------|
|<span data-ttu-id="e3fc4-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3fc4-124">Authorization</span></span>| <span data-ttu-id="e3fc4-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e3fc4-p105">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="e3fc4-127">承諾</span><span class="sxs-lookup"><span data-stu-id="e3fc4-127">Accept</span></span> | <span data-ttu-id="e3fc4-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e3fc4-128">application/json</span></span> |

## <a name="response"></a><span data-ttu-id="e3fc4-129">応答</span><span class="sxs-lookup"><span data-stu-id="e3fc4-129">Response</span></span>
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

## <a name="list-of-actionstatus"></a><span data-ttu-id="e3fc4-130">ActionStatus の一覧</span><span class="sxs-lookup"><span data-stu-id="e3fc4-130">List of actionStatus</span></span>

- <span data-ttu-id="e3fc4-131">要求、またはコマンドで作成された、処理を待機しています。</span><span class="sxs-lookup"><span data-stu-id="e3fc4-131">requesting, // Command has been created and is waiting to be processed</span></span>
- <span data-ttu-id="e3fc4-132">sentToTarget、またはターゲット ・ デバイスに送信されたコマンド/</span><span class="sxs-lookup"><span data-stu-id="e3fc4-132">sentToTarget, // Command has been sent to the target device</span></span>
- <span data-ttu-id="e3fc4-133">実行するとターゲット ・ デバイスは、コマンドの受信を確認し、実行しています。</span><span class="sxs-lookup"><span data-stu-id="e3fc4-133">executing, // Target device acknowledged receipt of the command and is executing it</span></span>
- <span data-ttu-id="e3fc4-134">完了すると、コマンドの実行が完了しました</span><span class="sxs-lookup"><span data-stu-id="e3fc4-134">completed, // Command execution completed</span></span>
- <span data-ttu-id="e3fc4-135">failedToSend、またはターゲット ・ デバイスにコマンドを送信するサービスが失敗したと</span><span class="sxs-lookup"><span data-stu-id="e3fc4-135">failedToSend, // Service failed to send command to target device</span></span>
- <span data-ttu-id="e3fc4-136">executionFailed、または、コマンドの実行に失敗しました</span><span class="sxs-lookup"><span data-stu-id="e3fc4-136">executionFailed, // Command execution failed</span></span>
- <span data-ttu-id="e3fc4-137">commandDropped、またはデバイスは ConnectedStandby の状態にある場合に、コマンドがクライアントによって削除/</span><span class="sxs-lookup"><span data-stu-id="e3fc4-137">commandDropped, // Command dropped by client if device is in ConnectedStandby state</span></span>
- <span data-ttu-id="e3fc4-138">取り消すには、//コマンドのキャンセル</span><span class="sxs-lookup"><span data-stu-id="e3fc4-138">cancel, // Cancel the command</span></span>
- <span data-ttu-id="e3fc4-139">キャンセルする、またはコマンドをキャンセルすると</span><span class="sxs-lookup"><span data-stu-id="e3fc4-139">cancelling, // Cancelling the command</span></span>
- <span data-ttu-id="e3fc4-140">キャンセルするには、//、コマンドは取り消されました</span><span class="sxs-lookup"><span data-stu-id="e3fc4-140">canceled, // Command has been cancelled</span></span>
- <span data-ttu-id="e3fc4-141">再試行、またはサービスがターゲットにコマンドを送信する再試行/</span><span class="sxs-lookup"><span data-stu-id="e3fc4-141">retry, // Service is retrying to send command to target</span></span>
- <span data-ttu-id="e3fc4-142">有効期限が切れた、またはコマンドの処理の有効期限を超過すると</span><span class="sxs-lookup"><span data-stu-id="e3fc4-142">expired, // Command processing exceeded expiry time</span></span>
- <span data-ttu-id="e3fc4-143">エラー、または内部またはコマンドの処理中にエラー</span><span class="sxs-lookup"><span data-stu-id="e3fc4-143">error, // Internal error while processing the command</span></span>
- <span data-ttu-id="e3fc4-144">カスタム/カスタム/ステータス</span><span class="sxs-lookup"><span data-stu-id="e3fc4-144">custom // Custom status</span></span>

## <a name="example"></a><span data-ttu-id="e3fc4-145">使用例</span><span class="sxs-lookup"><span data-stu-id="e3fc4-145">Example</span></span>

<span data-ttu-id="e3fc4-146">この例では、デバイスの ID とデバイスに発行されたコマンドの ID を必要があります。</span><span class="sxs-lookup"><span data-stu-id="e3fc4-146">In this example, you will need the ID of the device and the ID of the command that has been issued to a device.</span></span> <span data-ttu-id="e3fc4-147">GET を発行するときに ID が返されるデバイスの呼び出しの`/me/devices`の投稿を行うときに ID が返されるコマンドを呼び出すと`/me/devices/{id}/command`。</span><span class="sxs-lookup"><span data-stu-id="e3fc4-147">The device ID is returned when issuing a GET call to `/me/devices`, and the command ID is returned when doing a POST call on `/me/devices/{id}/command`.</span></span>

#### <a name="request"></a><span data-ttu-id="e3fc4-148">要求</span><span class="sxs-lookup"><span data-stu-id="e3fc4-148">Request</span></span>

<span data-ttu-id="e3fc4-149">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="e3fc4-149">The following example shows the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_command"
} -->
```http
GET me/devices/{id}/commands/{id}
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="e3fc4-150">応答</span><span class="sxs-lookup"><span data-stu-id="e3fc4-150">Response</span></span>

<span data-ttu-id="e3fc4-151">次の例は応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="e3fc4-151">The following example shows the response.</span></span>
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


## <a name="get-command-payload"></a><span data-ttu-id="e3fc4-152">コマンドのペイロードを取得します。</span><span class="sxs-lookup"><span data-stu-id="e3fc4-152">Get command payload</span></span>

<span data-ttu-id="e3fc4-153">デバイス上の特定のアクションの応答の内容を取得します。</span><span class="sxs-lookup"><span data-stu-id="e3fc4-153">Get a response payload for a specific action on a device.</span></span> <span data-ttu-id="e3fc4-154">応答の内容は、データを再度実行するために、アプリケーション サービスを照会するときに使用されます。</span><span class="sxs-lookup"><span data-stu-id="e3fc4-154">The response payload is used when querying an app service to carry data back.</span></span>


### <a name="permissions"></a><span data-ttu-id="e3fc4-155">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e3fc4-155">Permissions</span></span>

<span data-ttu-id="e3fc4-p108">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e3fc4-p108">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3fc4-158">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e3fc4-158">Permission type</span></span>      | <span data-ttu-id="e3fc4-159">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e3fc4-159">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e3fc4-160">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e3fc4-160">Delegated (work or school account)</span></span> | <span data-ttu-id="e3fc4-161">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e3fc4-161">Not supported.</span></span>    |
|<span data-ttu-id="e3fc4-162">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e3fc4-162">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3fc4-163">Device.Command</span><span class="sxs-lookup"><span data-stu-id="e3fc4-163">Device.Command</span></span>    |
|<span data-ttu-id="e3fc4-164">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e3fc4-164">Application</span></span> | <span data-ttu-id="e3fc4-165">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e3fc4-165">Not supported.</span></span> |

### <a name="http-request"></a><span data-ttu-id="e3fc4-166">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e3fc4-166">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices/{id}/command/{id}/responsePayload
```

### <a name="request-headers"></a><span data-ttu-id="e3fc4-167">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e3fc4-167">Request headers</span></span>

| <span data-ttu-id="e3fc4-168">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e3fc4-168">Header</span></span> |<span data-ttu-id="e3fc4-169">値</span><span class="sxs-lookup"><span data-stu-id="e3fc4-169">Value</span></span>
|:----|:------|
|<span data-ttu-id="e3fc4-170">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3fc4-170">Authorization</span></span>| <span data-ttu-id="e3fc4-p109">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e3fc4-p109">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="e3fc4-173">承諾</span><span class="sxs-lookup"><span data-stu-id="e3fc4-173">Accept</span></span> | <span data-ttu-id="e3fc4-174">application/json</span><span class="sxs-lookup"><span data-stu-id="e3fc4-174">application/json</span></span> |

### <a name="response"></a><span data-ttu-id="e3fc4-175">応答</span><span class="sxs-lookup"><span data-stu-id="e3fc4-175">Response</span></span>
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

### <a name="example"></a><span data-ttu-id="e3fc4-176">使用例</span><span class="sxs-lookup"><span data-stu-id="e3fc4-176">Example</span></span>

<span data-ttu-id="e3fc4-177">この例では、デバイスの ID とデバイスに発行されたコマンドの ID を必要があります。</span><span class="sxs-lookup"><span data-stu-id="e3fc4-177">In this example, you will need the ID of the device and the ID of the command that has been issued to a device.</span></span> <span data-ttu-id="e3fc4-178">に対して GET を発行するときに ID が返されるデバイスを呼び出す`/me/devices`の投稿を行うときに ID が返されるコマンドを呼び出すと`/me/devices/{id}/command`。</span><span class="sxs-lookup"><span data-stu-id="e3fc4-178">The device ID is returned when issuing a GET call on `/me/devices`, and the command ID is returned when doing a POST call on `/me/devices/{id}/command`.</span></span>

#### <a name="request"></a><span data-ttu-id="e3fc4-179">要求</span><span class="sxs-lookup"><span data-stu-id="e3fc4-179">Request</span></span>

<span data-ttu-id="e3fc4-180">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="e3fc4-180">The following example shows the request.</span></span>

<!-- { 
  "blockType": "ignored",
  "name": "get_command_payload"
} -->
```http
GET me/devices/{id}/commands/{id}
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="e3fc4-181">応答</span><span class="sxs-lookup"><span data-stu-id="e3fc4-181">Response</span></span>

<span data-ttu-id="e3fc4-182">次の例は応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="e3fc4-182">The following example shows the response.</span></span>

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
