---
title: デバイス コマンドを送信します。
description: 'この API は、Microsoft アカウントに関連付けられているデバイスのコマンドをプロジェクトのローマの機能を使用します。 GET の呼び出しを実行した後は`me/devices`、デバイスにコマンドを実行するデバイスの ID を渡します。 コマンドの 2 つの種類がサポートされている: LaunchURI と AppServices。 LaunchURI を使用している場合は、*型*と*ペイロード*のパラメーターを指定します。 AppService 呼び出しに指定します '
ms.openlocfilehash: bf330ab1234ef6ce22c6a43711621827b628a7ac
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070419"
---
# <a name="send-device-command"></a><span data-ttu-id="b426b-107">デバイス コマンドを送信します。</span><span class="sxs-lookup"><span data-stu-id="b426b-107">Send device command</span></span>

> <span data-ttu-id="b426b-108">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b426b-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b426b-109">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b426b-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b426b-110">この API は、Microsoft アカウントに関連付けられているデバイスのコマンドをプロジェクトのローマの機能を使用します。</span><span class="sxs-lookup"><span data-stu-id="b426b-110">This API enables Project Rome capabilities to command a device associated with a Microsoft account.</span></span> <span data-ttu-id="b426b-111">GET の呼び出しを実行した後は`me/devices`、デバイスにコマンドを実行するデバイスの ID を渡します。</span><span class="sxs-lookup"><span data-stu-id="b426b-111">After doing a GET call on `me/devices`, pass in the ID of the device to issue a command to your device.</span></span> <span data-ttu-id="b426b-112">コマンドの 2 つの種類がサポートされている: LaunchURI と AppServices。</span><span class="sxs-lookup"><span data-stu-id="b426b-112">Two types of commands are supported: LaunchURI and AppServices.</span></span> <span data-ttu-id="b426b-113">LaunchURI を使用している場合は、*型*と*ペイロード*のパラメーターを指定します。</span><span class="sxs-lookup"><span data-stu-id="b426b-113">If you're using LaunchURI, specify the *type* and *payload* parameters.</span></span> <span data-ttu-id="b426b-114">AppService 呼び出しには、*型*、*ペイロード*、 *packageFamilyName*、および*appServiceName*パラメーターを指定します。</span><span class="sxs-lookup"><span data-stu-id="b426b-114">For an AppService call, specify the *type*, *payload*, *packageFamilyName*, and *appServiceName* parameters.</span></span>

## <a name="permissions"></a><span data-ttu-id="b426b-115">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b426b-115">Permissions</span></span>

<span data-ttu-id="b426b-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b426b-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b426b-118">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b426b-118">Permission type</span></span>      | <span data-ttu-id="b426b-119">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b426b-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b426b-120">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b426b-120">Delegated (work or school account)</span></span> | <span data-ttu-id="b426b-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b426b-121">Not supported.</span></span>    |
|<span data-ttu-id="b426b-122">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b426b-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b426b-123">Device.Command</span><span class="sxs-lookup"><span data-stu-id="b426b-123">Device.Command</span></span>    |
|<span data-ttu-id="b426b-124">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b426b-124">Application</span></span> | <span data-ttu-id="b426b-125">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b426b-125">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b426b-126">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b426b-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST me/devices/{id}/commands
```

## <a name="request-headers"></a><span data-ttu-id="b426b-127">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b426b-127">Request headers</span></span>


| <span data-ttu-id="b426b-128">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b426b-128">Header</span></span> |<span data-ttu-id="b426b-129">値</span><span class="sxs-lookup"><span data-stu-id="b426b-129">Value</span></span>
|:----|:------|
|<span data-ttu-id="b426b-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="b426b-130">Authorization</span></span>| <span data-ttu-id="b426b-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b426b-p105">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="b426b-133">承諾</span><span class="sxs-lookup"><span data-stu-id="b426b-133">Accept</span></span> | <span data-ttu-id="b426b-134">application/json</span><span class="sxs-lookup"><span data-stu-id="b426b-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="b426b-135">要求本文</span><span class="sxs-lookup"><span data-stu-id="b426b-135">Request body</span></span>

<span data-ttu-id="b426b-136">要求の本文には、コマンドのプロパティの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="b426b-136">In the request body, supply a JSON representation of the command properties.</span></span>

```json
{
  "type": "appService",
  "payload": "payload-JSON",
  "packageFamilyName": "packageFamilyName",
  "appServiceName": "appServiceName",
  "postbackURI": "postbackURI"
}
```

## <a name="response"></a><span data-ttu-id="b426b-137">応答</span><span class="sxs-lookup"><span data-stu-id="b426b-137">Response</span></span>

```http
HTTP/1.1 201 OK
```

```json
{
  "id": "0",
  "status": "requesting",
  "type": "appService",
  "appServiceName": "appServiceName",
  "packageFamilyName": "packageFamilyName",
  "error": "null",
  "responsePayload": "null",
  "payload": "payload-JSON",
  "permissionTicket": "null",
  "postBackUri": "postbackURI"
}
```
## <a name="command-properties"></a><span data-ttu-id="b426b-138">コマンドのプロパティ</span><span class="sxs-lookup"><span data-stu-id="b426b-138">Command properties</span></span> 

|<span data-ttu-id="b426b-139">**名前**</span><span class="sxs-lookup"><span data-stu-id="b426b-139">**Name**</span></span>|<span data-ttu-id="b426b-140">**種類**</span><span class="sxs-lookup"><span data-stu-id="b426b-140">**Type**</span></span>|<span data-ttu-id="b426b-141">**説明**</span><span class="sxs-lookup"><span data-stu-id="b426b-141">**Description**</span></span>|
|:----|:------|:------|
|<span data-ttu-id="b426b-142">payload</span><span class="sxs-lookup"><span data-stu-id="b426b-142">payload</span></span> | <span data-ttu-id="b426b-143">microsoft.graph.json</span><span class="sxs-lookup"><span data-stu-id="b426b-143">microsoft.graph.json</span></span>| <span data-ttu-id="b426b-144">ペイロードのアプリケーション サービスに送信するか、デバイスの URI を起動します。</span><span class="sxs-lookup"><span data-stu-id="b426b-144">Payload to send to an app service or to launch a URI on a device.</span></span> |
|<span data-ttu-id="b426b-145">responsePayload</span><span class="sxs-lookup"><span data-stu-id="b426b-145">responsePayload</span></span> | <span data-ttu-id="b426b-146">microsoft.graph.json</span><span class="sxs-lookup"><span data-stu-id="b426b-146">microsoft.graph.json</span></span>| <span data-ttu-id="b426b-147">ペイロードは、ターゲット ・ デバイスから返されます。</span><span class="sxs-lookup"><span data-stu-id="b426b-147">Payload returned from target device.</span></span> |
|<span data-ttu-id="b426b-148">postBackURI</span><span class="sxs-lookup"><span data-stu-id="b426b-148">postBackURI</span></span> | <span data-ttu-id="b426b-149">String</span><span class="sxs-lookup"><span data-stu-id="b426b-149">String</span></span> | <span data-ttu-id="b426b-150">投稿は、更新の後続の通知を送信する URI をバックアップします。</span><span class="sxs-lookup"><span data-stu-id="b426b-150">Post back URI to send subsequent notifications of updates.</span></span> |
|<span data-ttu-id="b426b-151">packageFamilyName</span><span class="sxs-lookup"><span data-stu-id="b426b-151">packageFamilyName</span></span> | <span data-ttu-id="b426b-152">String</span><span class="sxs-lookup"><span data-stu-id="b426b-152">String</span></span> | <span data-ttu-id="b426b-153">Windows のアプリケーションのパッケージ ファミリ名。</span><span class="sxs-lookup"><span data-stu-id="b426b-153">Windows Package Family Name of application.</span></span> |
|<span data-ttu-id="b426b-154">appServiceName</span><span class="sxs-lookup"><span data-stu-id="b426b-154">appServiceName</span></span> | <span data-ttu-id="b426b-155">String</span><span class="sxs-lookup"><span data-stu-id="b426b-155">String</span></span> | <span data-ttu-id="b426b-156">対象のアプリケーションで定義されているアプリケーション サービスの名前です。</span><span class="sxs-lookup"><span data-stu-id="b426b-156">Name of app service defined by the target application.</span></span> <span data-ttu-id="b426b-157">場合は、アプリケーション サービスを起動する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b426b-157">Required if launching an app service.</span></span> |
|<span data-ttu-id="b426b-158">type</span><span class="sxs-lookup"><span data-stu-id="b426b-158">type</span></span>| <span data-ttu-id="b426b-159">String</span><span class="sxs-lookup"><span data-stu-id="b426b-159">String</span></span> | <span data-ttu-id="b426b-160">LaunchURI または AppService です。</span><span class="sxs-lookup"><span data-stu-id="b426b-160">LaunchURI or AppService.</span></span> |
|<span data-ttu-id="b426b-161">id</span><span class="sxs-lookup"><span data-stu-id="b426b-161">id</span></span>| <span data-ttu-id="b426b-162">String</span><span class="sxs-lookup"><span data-stu-id="b426b-162">String</span></span> | <span data-ttu-id="b426b-163">デバイスに送信されたコマンドの ID。</span><span class="sxs-lookup"><span data-stu-id="b426b-163">The ID of a command that has been sent to the device.</span></span> |
|<span data-ttu-id="b426b-164">actionStatus</span><span class="sxs-lookup"><span data-stu-id="b426b-164">actionStatus</span></span> | <span data-ttu-id="b426b-165">String</span><span class="sxs-lookup"><span data-stu-id="b426b-165">String</span></span> | <span data-ttu-id="b426b-166">コマンドの[ステータス](get-device-command-status.md)です。</span><span class="sxs-lookup"><span data-stu-id="b426b-166">The [status](get-device-command-status.md) of a command.</span></span> |
|<span data-ttu-id="b426b-167">エラー</span><span class="sxs-lookup"><span data-stu-id="b426b-167">error</span></span>| <span data-ttu-id="b426b-168">String</span><span class="sxs-lookup"><span data-stu-id="b426b-168">String</span></span>| <span data-ttu-id="b426b-169">ターゲット アプリケーションからの要求に関連付けられているエラーです。</span><span class="sxs-lookup"><span data-stu-id="b426b-169">Any errors associated with the request from the target application.</span></span> |

## <a name="launch-uri-example"></a><span data-ttu-id="b426b-170">URI の使用例を起動します。</span><span class="sxs-lookup"><span data-stu-id="b426b-170">Launch URI example</span></span>

<span data-ttu-id="b426b-171">LaunchURI 要求の例を次のとおりです。URI またはターゲット ・ デバイス上のアプリケーションが起動されます。</span><span class="sxs-lookup"><span data-stu-id="b426b-171">Here is an example of a LaunchURI request; it will launch a URI or an application on the target device.</span></span> <span data-ttu-id="b426b-172">URI またはアプリケーションを起動するには、デバイスの ID を使用して投稿を発行します (GET の呼び出しを行うから取得した`me/devices`)。</span><span class="sxs-lookup"><span data-stu-id="b426b-172">To launch a URI or an app, issue a POST using the ID of the device (obtained from doing a GET call on `me/devices`).</span></span> <span data-ttu-id="b426b-173">*型*パラメーターを*LaunchURI*に設定し、URI 値を指定して次のようにhttps://bing.com。</span><span class="sxs-lookup"><span data-stu-id="b426b-173">Set the *Type* parameters to *LaunchURI* and provide a URI value such as https://bing.com.</span></span>

#### <a name="request"></a><span data-ttu-id="b426b-174">要求</span><span class="sxs-lookup"><span data-stu-id="b426b-174">Request</span></span>

<span data-ttu-id="b426b-175">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b426b-175">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "post_command"
} -->

```http

POST me/devices/{id}/commands
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8

{ "type" : "LaunchUri", "payload" : {"uri":"https://bing.com"}}

```

#### <a name="response"></a><span data-ttu-id="b426b-176">応答</span><span class="sxs-lookup"><span data-stu-id="b426b-176">Response</span></span> 

<span data-ttu-id="b426b-177">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b426b-177">The following is an example of the response.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.commandobject",
  "isCollection": true
} -->

```http
HTTP/1.1 201 OK

{
  "id": "0158355AD4D680CC4E2994CC009EFFD7337D1B...",
  "status": "requesting",
  "type": null,
  "appServiceName": null,
  "packageFamilyName": null,
  "error": null,
  "permissionTicket": null,
  "postBackUri": null,
  "payload": {
    "uri": "https://bing.com"
  }
}

```


## <a name="app-service-example"></a><span data-ttu-id="b426b-178">アプリケーション サービスの例</span><span class="sxs-lookup"><span data-stu-id="b426b-178">App service example</span></span>

<span data-ttu-id="b426b-179">ここでは、デバイスで、アプリケーションのサービスのクエリの例です。</span><span class="sxs-lookup"><span data-stu-id="b426b-179">Here is an example of querying an app service on a device.</span></span> <span data-ttu-id="b426b-180">アプリケーション サービスを使用するデバイスの id を使用して POST 呼び出しを行う必要があります (GET の呼び出しを行うから取得した`me/devices`)。</span><span class="sxs-lookup"><span data-stu-id="b426b-180">To use an app service you must do a POST call using the id of the device (obtained from doing a GET call on `me/devices`).</span></span> <span data-ttu-id="b426b-181">次の例を使用するには、ターゲット ・ デバイスに[ローマのアプリケーション](https://aka.ms/romanapp)をインストールしてください。</span><span class="sxs-lookup"><span data-stu-id="b426b-181">To use the following example, you must install the [Rome app](https://aka.ms/romanapp) on your target device.</span></span>

<span data-ttu-id="b426b-182">呼び出しでは、いくつかの追加プロパティを設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b426b-182">Several additional properties must be set in the call.</span></span> <span data-ttu-id="b426b-183">*型*は、 *AppService*に設定する必要があります。、 *AppServiceName*は、アプリケーションで定義されているアプリケーション サービスの名前に設定する必要があります。、 *PackageFamilyName*は、アプリケーション マニフェスト、および*ペイロード*で定義されているパッケージのファミリ名を設定する必要があります。キーと呼び出し先のアプリケーション サービスの値を保持します。</span><span class="sxs-lookup"><span data-stu-id="b426b-183">*Type* must be set to *AppService*, *AppServiceName* must be set to the name of the app service defined in the application, *PackageFamilyName* must be set to the package family name defined in the app manifest, and *Payload* holds the keys and values for the service you are calling within the target application.</span></span>

#### <a name="request"></a><span data-ttu-id="b426b-184">要求</span><span class="sxs-lookup"><span data-stu-id="b426b-184">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "post_command_2"
} -->

```http

POST me/devices/{id}/commands
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8

{
  "type" : "AppService",
  "appServiceName" : "com.microsoft.test.cdppingpongservice",
  "packageFamilyName" : "5085ShawnHenry.RomanTestApp_jsjw7knzsgcce",
  "payload" : {
    "Type":"Toast","Title":"Hello","Subtitle":"World!"}
  }
```

#### <a name="response"></a><span data-ttu-id="b426b-185">応答</span><span class="sxs-lookup"><span data-stu-id="b426b-185">Response</span></span>

<span data-ttu-id="b426b-186">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b426b-186">The following is an example of the response.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.commandobject",
  "isCollection": true
} -->

```http
HTTP/1.1 201 OK

{
  "id": "0158355AD4D680CC4E2994CC009EFFD7EADA8307E96FF1C8D19B..",
  "status": "requesting",
  "type": null,
  "appServiceName": "com.microsoft.randomnumbergenerator",
  "packageFamilyName": "Microsoft.SDKSamples.AppServicesProvider.CS_8wekyb3d8bbwe",
  "error": null,
  "permissionTicket": null,
  "postBackUri": null,
  "payload": {
    "Type": "Toast",
    "Title": "Hello",
    "Subtitle": "World!"
  }
}
```
