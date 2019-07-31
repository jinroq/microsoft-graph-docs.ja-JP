---
title: デバイス コマンドの状態を取得する
description: デバイス上のコマンドの状態を取得します。 状態コードの完全な一覧については、「actionStatus の一覧」を参照してください。
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: 74104859b0621e51c0af9eced15912632fe5b9fb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35954306"
---
# <a name="get-device-command-status"></a><span data-ttu-id="72f52-104">デバイス コマンドの状態を取得する</span><span class="sxs-lookup"><span data-stu-id="72f52-104">Get device command status</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72f52-105">デバイス上のコマンドの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="72f52-105">Get the status of a command on a device.</span></span> <span data-ttu-id="72f52-106">状態コードの完全な一覧については、「 [actionStatus の一覧](#list-of-actionstatus)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="72f52-106">For the  full list of status codes, see [List of actionStatus](#list-of-actionstatus).</span></span>

## <a name="permissions"></a><span data-ttu-id="72f52-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="72f52-107">Permissions</span></span>

<span data-ttu-id="72f52-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="72f52-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72f52-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="72f52-110">Permission type</span></span>      | <span data-ttu-id="72f52-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="72f52-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="72f52-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="72f52-112">Delegated (work or school account)</span></span> | <span data-ttu-id="72f52-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="72f52-113">Not supported.</span></span>    |
|<span data-ttu-id="72f52-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="72f52-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72f52-115">Device.Command</span><span class="sxs-lookup"><span data-stu-id="72f52-115">Device.Command</span></span>    |
|<span data-ttu-id="72f52-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="72f52-116">Application</span></span> | <span data-ttu-id="72f52-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="72f52-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="72f52-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="72f52-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices/{id}/commands/{id}
```

## <a name="request-headers"></a><span data-ttu-id="72f52-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="72f52-119">Request headers</span></span>

| <span data-ttu-id="72f52-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="72f52-120">Header</span></span> |<span data-ttu-id="72f52-121">値</span><span class="sxs-lookup"><span data-stu-id="72f52-121">Value</span></span>
|:----|:------|
|<span data-ttu-id="72f52-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="72f52-122">Authorization</span></span>| <span data-ttu-id="72f52-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="72f52-p104">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="72f52-125">承諾</span><span class="sxs-lookup"><span data-stu-id="72f52-125">Accept</span></span> | <span data-ttu-id="72f52-126">application/json</span><span class="sxs-lookup"><span data-stu-id="72f52-126">application/json</span></span> |

## <a name="response"></a><span data-ttu-id="72f52-127">応答</span><span class="sxs-lookup"><span data-stu-id="72f52-127">Response</span></span>
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

## <a name="list-of-actionstatus"></a><span data-ttu-id="72f52-128">ActionStatus の一覧</span><span class="sxs-lookup"><span data-stu-id="72f52-128">List of actionStatus</span></span>

- <span data-ttu-id="72f52-129">要求のコマンドが作成され、処理を待っています</span><span class="sxs-lookup"><span data-stu-id="72f52-129">requesting, // Command has been created and is waiting to be processed</span></span>
- <span data-ttu-id="72f52-130">送信ターゲット、//コマンドがターゲットデバイスに送信されました</span><span class="sxs-lookup"><span data-stu-id="72f52-130">sentToTarget, // Command has been sent to the target device</span></span>
- <span data-ttu-id="72f52-131">コマンドを実行中で、ターゲットデバイスの確認済み受信を実行中です。</span><span class="sxs-lookup"><span data-stu-id="72f52-131">executing, // Target device acknowledged receipt of the command and is executing it</span></span>
- <span data-ttu-id="72f52-132">完了、//コマンドの実行が完了</span><span class="sxs-lookup"><span data-stu-id="72f52-132">completed, // Command execution completed</span></span>
- <span data-ttu-id="72f52-133">失敗/送信、//サービスがターゲットデバイスにコマンドを送信できませんでした</span><span class="sxs-lookup"><span data-stu-id="72f52-133">failedToSend, // Service failed to send command to target device</span></span>
- <span data-ttu-id="72f52-134">executionFailed、//コマンドの実行に失敗しました</span><span class="sxs-lookup"><span data-stu-id="72f52-134">executionFailed, // Command execution failed</span></span>
- <span data-ttu-id="72f52-135">デバイスが ConnectedStandby の状態にある場合、コマンドはクライアントによってドロップされています。</span><span class="sxs-lookup"><span data-stu-id="72f52-135">commandDropped, // Command dropped by client if device is in ConnectedStandby state</span></span>
- <span data-ttu-id="72f52-136">cancel、コマンドをキャンセルする</span><span class="sxs-lookup"><span data-stu-id="72f52-136">cancel, // Cancel the command</span></span>
- <span data-ttu-id="72f52-137">コマンドをキャンセルする、//キャンセルする</span><span class="sxs-lookup"><span data-stu-id="72f52-137">cancelling, // Cancelling the command</span></span>
- <span data-ttu-id="72f52-138">取り消し済み//コマンドは取り消されました</span><span class="sxs-lookup"><span data-stu-id="72f52-138">canceled, // Command has been cancelled</span></span>
- <span data-ttu-id="72f52-139">再試行、//サービスはターゲットへのコマンドの送信を再試行しています</span><span class="sxs-lookup"><span data-stu-id="72f52-139">retry, // Service is retrying to send command to target</span></span>
- <span data-ttu-id="72f52-140">期限切れ、コマンド処理が有効期限を超過しました</span><span class="sxs-lookup"><span data-stu-id="72f52-140">expired, // Command processing exceeded expiry time</span></span>
- <span data-ttu-id="72f52-141">エラー、コマンドの処理中に内部エラーが発生しました</span><span class="sxs-lookup"><span data-stu-id="72f52-141">error, // Internal error while processing the command</span></span>
- <span data-ttu-id="72f52-142">カスタム/カスタム状態</span><span class="sxs-lookup"><span data-stu-id="72f52-142">custom // Custom status</span></span>

## <a name="example"></a><span data-ttu-id="72f52-143">例</span><span class="sxs-lookup"><span data-stu-id="72f52-143">Example</span></span>

<span data-ttu-id="72f52-144">この例では、デバイスの ID と、デバイスに発行されたコマンドの ID が必要になります。</span><span class="sxs-lookup"><span data-stu-id="72f52-144">In this example, you will need the ID of the device and the ID of the command that has been issued to a device.</span></span> <span data-ttu-id="72f52-145">デバイス ID は GET 呼び出し`/me/devices`を発行したときに返され、に対して`/me/devices/{id}/command`POST 呼び出しを実行すると、コマンド id が返されます。</span><span class="sxs-lookup"><span data-stu-id="72f52-145">The device ID is returned when issuing a GET call to `/me/devices`, and the command ID is returned when doing a POST call on `/me/devices/{id}/command`.</span></span>

#### <a name="request"></a><span data-ttu-id="72f52-146">要求</span><span class="sxs-lookup"><span data-stu-id="72f52-146">Request</span></span>

<span data-ttu-id="72f52-147">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="72f52-147">The following example shows the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_command"
} -->
```http
GET me/devices/{id}/commands/{id}
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="72f52-148">応答</span><span class="sxs-lookup"><span data-stu-id="72f52-148">Response</span></span>

<span data-ttu-id="72f52-149">次の例は応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="72f52-149">The following example shows the response.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.command",
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


## <a name="get-command-payload"></a><span data-ttu-id="72f52-150">コマンドペイロードの取得</span><span class="sxs-lookup"><span data-stu-id="72f52-150">Get command payload</span></span>

<span data-ttu-id="72f52-151">デバイス上の特定のアクションの応答ペイロードを取得します。</span><span class="sxs-lookup"><span data-stu-id="72f52-151">Get a response payload for a specific action on a device.</span></span> <span data-ttu-id="72f52-152">応答ペイロードは、アプリケーションサービスに対してクエリを実行してデータを返すときに使用されます。</span><span class="sxs-lookup"><span data-stu-id="72f52-152">The response payload is used when querying an app service to carry data back.</span></span>


### <a name="permissions"></a><span data-ttu-id="72f52-153">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="72f52-153">Permissions</span></span>

<span data-ttu-id="72f52-p107">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="72f52-p107">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72f52-156">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="72f52-156">Permission type</span></span>      | <span data-ttu-id="72f52-157">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="72f52-157">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="72f52-158">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="72f52-158">Delegated (work or school account)</span></span> | <span data-ttu-id="72f52-159">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="72f52-159">Not supported.</span></span>    |
|<span data-ttu-id="72f52-160">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="72f52-160">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72f52-161">Device.Command</span><span class="sxs-lookup"><span data-stu-id="72f52-161">Device.Command</span></span>    |
|<span data-ttu-id="72f52-162">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="72f52-162">Application</span></span> | <span data-ttu-id="72f52-163">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="72f52-163">Not supported.</span></span> |

### <a name="http-request"></a><span data-ttu-id="72f52-164">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="72f52-164">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices/{id}/command/{id}/responsePayload
```

### <a name="request-headers"></a><span data-ttu-id="72f52-165">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="72f52-165">Request headers</span></span>

| <span data-ttu-id="72f52-166">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="72f52-166">Header</span></span> |<span data-ttu-id="72f52-167">値</span><span class="sxs-lookup"><span data-stu-id="72f52-167">Value</span></span>
|:----|:------|
|<span data-ttu-id="72f52-168">Authorization</span><span class="sxs-lookup"><span data-stu-id="72f52-168">Authorization</span></span>| <span data-ttu-id="72f52-p108">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="72f52-p108">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="72f52-171">承諾</span><span class="sxs-lookup"><span data-stu-id="72f52-171">Accept</span></span> | <span data-ttu-id="72f52-172">application/json</span><span class="sxs-lookup"><span data-stu-id="72f52-172">application/json</span></span> |

### <a name="response"></a><span data-ttu-id="72f52-173">応答</span><span class="sxs-lookup"><span data-stu-id="72f52-173">Response</span></span>
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

### <a name="example"></a><span data-ttu-id="72f52-174">例</span><span class="sxs-lookup"><span data-stu-id="72f52-174">Example</span></span>

<span data-ttu-id="72f52-175">この例では、デバイスの ID と、デバイスに発行されたコマンドの ID が必要になります。</span><span class="sxs-lookup"><span data-stu-id="72f52-175">In this example, you will need the ID of the device and the ID of the command that has been issued to a device.</span></span> <span data-ttu-id="72f52-176">デバイス ID は GET 呼び出し`/me/devices`を発行したときに返され、に対して`/me/devices/{id}/command`POST 呼び出しを実行すると、コマンド id が返されます。</span><span class="sxs-lookup"><span data-stu-id="72f52-176">The device ID is returned when issuing a GET call on `/me/devices`, and the command ID is returned when doing a POST call on `/me/devices/{id}/command`.</span></span>

#### <a name="request"></a><span data-ttu-id="72f52-177">要求</span><span class="sxs-lookup"><span data-stu-id="72f52-177">Request</span></span>

<span data-ttu-id="72f52-178">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="72f52-178">The following example shows the request.</span></span>

<!-- { 
  "blockType": "ignored",
  "name": "get_command_payload"
} -->
```http
GET me/devices/{id}/commands/{id}
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="72f52-179">応答</span><span class="sxs-lookup"><span data-stu-id="72f52-179">Response</span></span>

<span data-ttu-id="72f52-180">次の例は応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="72f52-180">The following example shows the response.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.command",
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
