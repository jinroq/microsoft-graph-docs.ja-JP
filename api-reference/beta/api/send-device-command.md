---
title: デバイス コマンドを送信します。
description: 'この API は、Microsoft アカウントに関連付けられているデバイスのコマンドをプロジェクトのローマの機能を使用します。 GET の呼び出しを実行した後は`me/devices`、デバイスにコマンドを実行するデバイスの ID を渡します。 コマンドの 2 つの種類がサポートされている: LaunchURI と AppServices。 LaunchURI を使用している場合は、*型*と*ペイロード*のパラメーターを指定します。 AppService 呼び出しに指定します '
localization_priority: Normal
ms.openlocfilehash: d0c25200933a4a87a66349e457c500c496272b08
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526243"
---
# <a name="send-device-command"></a><span data-ttu-id="541ca-107">デバイス コマンドを送信します。</span><span class="sxs-lookup"><span data-stu-id="541ca-107">Send device command</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="541ca-108">この API は、Microsoft アカウントに関連付けられているデバイスのコマンドをプロジェクトのローマの機能を使用します。</span><span class="sxs-lookup"><span data-stu-id="541ca-108">This API enables Project Rome capabilities to command a device associated with a Microsoft account.</span></span> <span data-ttu-id="541ca-109">GET の呼び出しを実行した後は`me/devices`、デバイスにコマンドを実行するデバイスの ID を渡します。</span><span class="sxs-lookup"><span data-stu-id="541ca-109">After doing a GET call on `me/devices`, pass in the ID of the device to issue a command to your device.</span></span> <span data-ttu-id="541ca-110">コマンドの 2 つの種類がサポートされている: LaunchURI と AppServices。</span><span class="sxs-lookup"><span data-stu-id="541ca-110">Two types of commands are supported: LaunchURI and AppServices.</span></span> <span data-ttu-id="541ca-111">LaunchURI を使用している場合は、*型*と*ペイロード*のパラメーターを指定します。</span><span class="sxs-lookup"><span data-stu-id="541ca-111">If you're using LaunchURI, specify the *type* and *payload* parameters.</span></span> <span data-ttu-id="541ca-112">AppService 呼び出しには、*型*、*ペイロード*、 *packageFamilyName*、および*appServiceName*パラメーターを指定します。</span><span class="sxs-lookup"><span data-stu-id="541ca-112">For an AppService call, specify the *type*, *payload*, *packageFamilyName*, and *appServiceName* parameters.</span></span>

## <a name="permissions"></a><span data-ttu-id="541ca-113">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="541ca-113">Permissions</span></span>

<span data-ttu-id="541ca-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="541ca-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="541ca-116">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="541ca-116">Permission type</span></span>      | <span data-ttu-id="541ca-117">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="541ca-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="541ca-118">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="541ca-118">Delegated (work or school account)</span></span> | <span data-ttu-id="541ca-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="541ca-119">Not supported.</span></span>    |
|<span data-ttu-id="541ca-120">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="541ca-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="541ca-121">Device.Command</span><span class="sxs-lookup"><span data-stu-id="541ca-121">Device.Command</span></span>    |
|<span data-ttu-id="541ca-122">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="541ca-122">Application</span></span> | <span data-ttu-id="541ca-123">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="541ca-123">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="541ca-124">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="541ca-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST me/devices/{id}/commands
```

## <a name="request-headers"></a><span data-ttu-id="541ca-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="541ca-125">Request headers</span></span>


| <span data-ttu-id="541ca-126">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="541ca-126">Header</span></span> |<span data-ttu-id="541ca-127">値</span><span class="sxs-lookup"><span data-stu-id="541ca-127">Value</span></span>
|:----|:------|
|<span data-ttu-id="541ca-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="541ca-128">Authorization</span></span>| <span data-ttu-id="541ca-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="541ca-p104">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="541ca-131">承諾</span><span class="sxs-lookup"><span data-stu-id="541ca-131">Accept</span></span> | <span data-ttu-id="541ca-132">application/json</span><span class="sxs-lookup"><span data-stu-id="541ca-132">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="541ca-133">要求本文</span><span class="sxs-lookup"><span data-stu-id="541ca-133">Request body</span></span>

<span data-ttu-id="541ca-134">要求の本文には、コマンドのプロパティの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="541ca-134">In the request body, supply a JSON representation of the command properties.</span></span>

```json
{
  "type": "appService",
  "payload": "payload-JSON",
  "packageFamilyName": "packageFamilyName",
  "appServiceName": "appServiceName",
  "postbackURI": "postbackURI"
}
```

## <a name="response"></a><span data-ttu-id="541ca-135">応答</span><span class="sxs-lookup"><span data-stu-id="541ca-135">Response</span></span>

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
## <a name="command-properties"></a><span data-ttu-id="541ca-136">Command Properties</span><span class="sxs-lookup"><span data-stu-id="541ca-136">Command properties</span></span> 

|<span data-ttu-id="541ca-137">**Name**</span><span class="sxs-lookup"><span data-stu-id="541ca-137">**Name**</span></span>|<span data-ttu-id="541ca-138">**型**</span><span class="sxs-lookup"><span data-stu-id="541ca-138">**Type**</span></span>|<span data-ttu-id="541ca-139">**説明**</span><span class="sxs-lookup"><span data-stu-id="541ca-139">**Description**</span></span>|
|:----|:------|:------|
|<span data-ttu-id="541ca-140">payload</span><span class="sxs-lookup"><span data-stu-id="541ca-140">payload</span></span> | <span data-ttu-id="541ca-141">microsoft.graph.json</span><span class="sxs-lookup"><span data-stu-id="541ca-141">microsoft.graph.json</span></span>| <span data-ttu-id="541ca-142">ペイロードのアプリケーション サービスに送信するか、デバイスの URI を起動します。</span><span class="sxs-lookup"><span data-stu-id="541ca-142">Payload to send to an app service or to launch a URI on a device.</span></span> |
|<span data-ttu-id="541ca-143">responsePayload</span><span class="sxs-lookup"><span data-stu-id="541ca-143">responsePayload</span></span> | <span data-ttu-id="541ca-144">microsoft.graph.json</span><span class="sxs-lookup"><span data-stu-id="541ca-144">microsoft.graph.json</span></span>| <span data-ttu-id="541ca-145">ペイロードは、ターゲット ・ デバイスから返されます。</span><span class="sxs-lookup"><span data-stu-id="541ca-145">Payload returned from target device.</span></span> |
|<span data-ttu-id="541ca-146">postBackURI</span><span class="sxs-lookup"><span data-stu-id="541ca-146">postBackURI</span></span> | <span data-ttu-id="541ca-147">String</span><span class="sxs-lookup"><span data-stu-id="541ca-147">String</span></span> | <span data-ttu-id="541ca-148">投稿は、更新の後続の通知を送信する URI をバックアップします。</span><span class="sxs-lookup"><span data-stu-id="541ca-148">Post back URI to send subsequent notifications of updates.</span></span> |
|<span data-ttu-id="541ca-149">packageFamilyName</span><span class="sxs-lookup"><span data-stu-id="541ca-149">packageFamilyName</span></span> | <span data-ttu-id="541ca-150">String</span><span class="sxs-lookup"><span data-stu-id="541ca-150">String</span></span> | <span data-ttu-id="541ca-151">Windows のアプリケーションのパッケージ ファミリ名。</span><span class="sxs-lookup"><span data-stu-id="541ca-151">Windows Package Family Name of application.</span></span> |
|<span data-ttu-id="541ca-152">appServiceName</span><span class="sxs-lookup"><span data-stu-id="541ca-152">appServiceName</span></span> | <span data-ttu-id="541ca-153">String</span><span class="sxs-lookup"><span data-stu-id="541ca-153">String</span></span> | <span data-ttu-id="541ca-154">対象のアプリケーションで定義されているアプリケーション サービスの名前です。</span><span class="sxs-lookup"><span data-stu-id="541ca-154">Name of app service defined by the target application.</span></span> <span data-ttu-id="541ca-155">場合は、アプリケーション サービスを起動する必要があります。</span><span class="sxs-lookup"><span data-stu-id="541ca-155">Required if launching an app service.</span></span> |
|<span data-ttu-id="541ca-156">type</span><span class="sxs-lookup"><span data-stu-id="541ca-156">type</span></span>| <span data-ttu-id="541ca-157">String</span><span class="sxs-lookup"><span data-stu-id="541ca-157">String</span></span> | <span data-ttu-id="541ca-158">LaunchURI または AppService です。</span><span class="sxs-lookup"><span data-stu-id="541ca-158">LaunchURI or AppService.</span></span> |
|<span data-ttu-id="541ca-159">id</span><span class="sxs-lookup"><span data-stu-id="541ca-159">id</span></span>| <span data-ttu-id="541ca-160">String</span><span class="sxs-lookup"><span data-stu-id="541ca-160">String</span></span> | <span data-ttu-id="541ca-161">デバイスに送信されたコマンドの ID。</span><span class="sxs-lookup"><span data-stu-id="541ca-161">The ID of a command that has been sent to the device.</span></span> |
|<span data-ttu-id="541ca-162">actionStatus</span><span class="sxs-lookup"><span data-stu-id="541ca-162">actionStatus</span></span> | <span data-ttu-id="541ca-163">String</span><span class="sxs-lookup"><span data-stu-id="541ca-163">String</span></span> | <span data-ttu-id="541ca-164">コマンドの[ステータス](get-device-command-status.md)です。</span><span class="sxs-lookup"><span data-stu-id="541ca-164">The [status](get-device-command-status.md) of a command.</span></span> |
|<span data-ttu-id="541ca-165">エラー</span><span class="sxs-lookup"><span data-stu-id="541ca-165">error</span></span>| <span data-ttu-id="541ca-166">String</span><span class="sxs-lookup"><span data-stu-id="541ca-166">String</span></span>| <span data-ttu-id="541ca-167">ターゲット アプリケーションからの要求に関連付けられているエラーです。</span><span class="sxs-lookup"><span data-stu-id="541ca-167">Any errors associated with the request from the target application.</span></span> |

## <a name="launch-uri-example"></a><span data-ttu-id="541ca-168">URI の使用例を起動します。</span><span class="sxs-lookup"><span data-stu-id="541ca-168">Launch URI example</span></span>

<span data-ttu-id="541ca-169">LaunchURI 要求の例を次のとおりです。URI またはターゲット ・ デバイス上のアプリケーションが起動されます。</span><span class="sxs-lookup"><span data-stu-id="541ca-169">Here is an example of a LaunchURI request; it will launch a URI or an application on the target device.</span></span> <span data-ttu-id="541ca-170">URI またはアプリケーションを起動するには、デバイスの ID を使用して投稿を発行します (GET の呼び出しを行うから取得した`me/devices`)。</span><span class="sxs-lookup"><span data-stu-id="541ca-170">To launch a URI or an app, issue a POST using the ID of the device (obtained from doing a GET call on `me/devices`).</span></span> <span data-ttu-id="541ca-171">*型*パラメーターを*LaunchURI*に設定し、URI 値を指定して次のようにhttps://bing.com。</span><span class="sxs-lookup"><span data-stu-id="541ca-171">Set the *Type* parameters to *LaunchURI* and provide a URI value such as https://bing.com.</span></span>

#### <a name="request"></a><span data-ttu-id="541ca-172">要求</span><span class="sxs-lookup"><span data-stu-id="541ca-172">Request</span></span>

<span data-ttu-id="541ca-173">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="541ca-173">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="541ca-174">応答</span><span class="sxs-lookup"><span data-stu-id="541ca-174">Response</span></span> 

<span data-ttu-id="541ca-175">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="541ca-175">The following is an example of the response.</span></span>

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


## <a name="app-service-example"></a><span data-ttu-id="541ca-176">アプリケーション サービスの例</span><span class="sxs-lookup"><span data-stu-id="541ca-176">App service example</span></span>

<span data-ttu-id="541ca-177">ここでは、デバイスで、アプリケーションのサービスのクエリの例です。</span><span class="sxs-lookup"><span data-stu-id="541ca-177">Here is an example of querying an app service on a device.</span></span> <span data-ttu-id="541ca-178">アプリケーション サービスを使用するデバイスの id を使用して POST 呼び出しを行う必要があります (GET の呼び出しを行うから取得した`me/devices`)。</span><span class="sxs-lookup"><span data-stu-id="541ca-178">To use an app service you must do a POST call using the id of the device (obtained from doing a GET call on `me/devices`).</span></span> <span data-ttu-id="541ca-179">次の例を使用するには、ターゲット ・ デバイスに[ローマのアプリケーション](https://aka.ms/romanapp)をインストールしてください。</span><span class="sxs-lookup"><span data-stu-id="541ca-179">To use the following example, you must install the [Rome app](https://aka.ms/romanapp) on your target device.</span></span>

<span data-ttu-id="541ca-180">呼び出しでは、いくつかの追加プロパティを設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="541ca-180">Several additional properties must be set in the call.</span></span> <span data-ttu-id="541ca-181">*型*は、 *AppService*に設定する必要があります。、 *AppServiceName*は、アプリケーションで定義されているアプリケーション サービスの名前に設定する必要があります。、 *PackageFamilyName*は、アプリケーション マニフェスト、および*ペイロード*で定義されているパッケージのファミリ名を設定する必要があります。キーと呼び出し先のアプリケーション サービスの値を保持します。</span><span class="sxs-lookup"><span data-stu-id="541ca-181">*Type* must be set to *AppService*, *AppServiceName* must be set to the name of the app service defined in the application, *PackageFamilyName* must be set to the package family name defined in the app manifest, and *Payload* holds the keys and values for the service you are calling within the target application.</span></span>

#### <a name="request"></a><span data-ttu-id="541ca-182">要求</span><span class="sxs-lookup"><span data-stu-id="541ca-182">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="541ca-183">応答</span><span class="sxs-lookup"><span data-stu-id="541ca-183">Response</span></span>

<span data-ttu-id="541ca-184">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="541ca-184">The following is an example of the response.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/send-device-command.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
