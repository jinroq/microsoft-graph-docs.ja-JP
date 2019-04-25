---
title: デバイス コマンドを送信する
description: 'この API を使用すると、Project ローマ機能を使用して、Microsoft アカウントに関連付けられているデバイスにコマンドを実行できます。 GET 呼び出しを実行した`me/devices`後、デバイスにコマンドを発行するデバイスの ID を渡します。 launchuri と appservices という2種類のコマンドがサポートされています。 launchuri を使用している場合は、 *type*パラメーターと*payload*パラメーターを指定します。 AppService の呼び出しの場合は、 '
localization_priority: Normal
ms.openlocfilehash: d0c25200933a4a87a66349e457c500c496272b08
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32537530"
---
# <a name="send-device-command"></a><span data-ttu-id="5a66c-107">デバイス コマンドを送信する</span><span class="sxs-lookup"><span data-stu-id="5a66c-107">Send device command</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a66c-108">この API を使用すると、Project ローマ機能を使用して、Microsoft アカウントに関連付けられているデバイスにコマンドを実行できます。</span><span class="sxs-lookup"><span data-stu-id="5a66c-108">This API enables Project Rome capabilities to command a device associated with a Microsoft account.</span></span> <span data-ttu-id="5a66c-109">GET 呼び出しを実行した`me/devices`後、デバイスにコマンドを発行するデバイスの ID を渡します。</span><span class="sxs-lookup"><span data-stu-id="5a66c-109">After doing a GET call on `me/devices`, pass in the ID of the device to issue a command to your device.</span></span> <span data-ttu-id="5a66c-110">launchuri と appservices という2種類のコマンドがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="5a66c-110">Two types of commands are supported: LaunchURI and AppServices.</span></span> <span data-ttu-id="5a66c-111">launchuri を使用している場合は、 *type*パラメーターと*payload*パラメーターを指定します。</span><span class="sxs-lookup"><span data-stu-id="5a66c-111">If you're using LaunchURI, specify the *type* and *payload* parameters.</span></span> <span data-ttu-id="5a66c-112">AppService の呼び出しの場合は、 *type*、 *payload*、 *efamilyname*、 *appservicename*の各パラメーターを指定します。</span><span class="sxs-lookup"><span data-stu-id="5a66c-112">For an AppService call, specify the *type*, *payload*, *packageFamilyName*, and *appServiceName* parameters.</span></span>

## <a name="permissions"></a><span data-ttu-id="5a66c-113">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5a66c-113">Permissions</span></span>

<span data-ttu-id="5a66c-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5a66c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5a66c-116">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5a66c-116">Permission type</span></span>      | <span data-ttu-id="5a66c-117">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5a66c-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5a66c-118">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5a66c-118">Delegated (work or school account)</span></span> | <span data-ttu-id="5a66c-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5a66c-119">Not supported.</span></span>    |
|<span data-ttu-id="5a66c-120">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5a66c-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a66c-121">Device.Command</span><span class="sxs-lookup"><span data-stu-id="5a66c-121">Device.Command</span></span>    |
|<span data-ttu-id="5a66c-122">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5a66c-122">Application</span></span> | <span data-ttu-id="5a66c-123">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5a66c-123">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5a66c-124">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5a66c-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST me/devices/{id}/commands
```

## <a name="request-headers"></a><span data-ttu-id="5a66c-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5a66c-125">Request headers</span></span>


| <span data-ttu-id="5a66c-126">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5a66c-126">Header</span></span> |<span data-ttu-id="5a66c-127">値</span><span class="sxs-lookup"><span data-stu-id="5a66c-127">Value</span></span>
|:----|:------|
|<span data-ttu-id="5a66c-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a66c-128">Authorization</span></span>| <span data-ttu-id="5a66c-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5a66c-p104">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="5a66c-131">承諾</span><span class="sxs-lookup"><span data-stu-id="5a66c-131">Accept</span></span> | <span data-ttu-id="5a66c-132">application/json</span><span class="sxs-lookup"><span data-stu-id="5a66c-132">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="5a66c-133">要求本文</span><span class="sxs-lookup"><span data-stu-id="5a66c-133">Request body</span></span>

<span data-ttu-id="5a66c-134">要求本文で、コマンドプロパティの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="5a66c-134">In the request body, supply a JSON representation of the command properties.</span></span>

```json
{
  "type": "appService",
  "payload": "payload-JSON",
  "packageFamilyName": "packageFamilyName",
  "appServiceName": "appServiceName",
  "postbackURI": "postbackURI"
}
```

## <a name="response"></a><span data-ttu-id="5a66c-135">応答</span><span class="sxs-lookup"><span data-stu-id="5a66c-135">Response</span></span>

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
## <a name="command-properties"></a><span data-ttu-id="5a66c-136">コマンドのプロパティ</span><span class="sxs-lookup"><span data-stu-id="5a66c-136">Command properties</span></span> 

|<span data-ttu-id="5a66c-137">**名前**</span><span class="sxs-lookup"><span data-stu-id="5a66c-137">**Name**</span></span>|<span data-ttu-id="5a66c-138">**Type**</span><span class="sxs-lookup"><span data-stu-id="5a66c-138">**Type**</span></span>|<span data-ttu-id="5a66c-139">**説明**</span><span class="sxs-lookup"><span data-stu-id="5a66c-139">**Description**</span></span>|
|:----|:------|:------|
|<span data-ttu-id="5a66c-140">payload</span><span class="sxs-lookup"><span data-stu-id="5a66c-140">payload</span></span> | <span data-ttu-id="5a66c-141">microsoft graph</span><span class="sxs-lookup"><span data-stu-id="5a66c-141">microsoft.graph.json</span></span>| <span data-ttu-id="5a66c-142">アプリサービスに送信するペイロード、またはデバイスで URI を起動するためのペイロード。</span><span class="sxs-lookup"><span data-stu-id="5a66c-142">Payload to send to an app service or to launch a URI on a device.</span></span> |
|<span data-ttu-id="5a66c-143">responsepayload</span><span class="sxs-lookup"><span data-stu-id="5a66c-143">responsePayload</span></span> | <span data-ttu-id="5a66c-144">microsoft graph</span><span class="sxs-lookup"><span data-stu-id="5a66c-144">microsoft.graph.json</span></span>| <span data-ttu-id="5a66c-145">ターゲットデバイスから返されたペイロード。</span><span class="sxs-lookup"><span data-stu-id="5a66c-145">Payload returned from target device.</span></span> |
|<span data-ttu-id="5a66c-146">postBackURI</span><span class="sxs-lookup"><span data-stu-id="5a66c-146">postBackURI</span></span> | <span data-ttu-id="5a66c-147">String</span><span class="sxs-lookup"><span data-stu-id="5a66c-147">String</span></span> | <span data-ttu-id="5a66c-148">今後の更新通知を送信するための URI をポストバックします。</span><span class="sxs-lookup"><span data-stu-id="5a66c-148">Post back URI to send subsequent notifications of updates.</span></span> |
|<span data-ttu-id="5a66c-149">パッケージ efamilyname</span><span class="sxs-lookup"><span data-stu-id="5a66c-149">packageFamilyName</span></span> | <span data-ttu-id="5a66c-150">String</span><span class="sxs-lookup"><span data-stu-id="5a66c-150">String</span></span> | <span data-ttu-id="5a66c-151">Windows パッケージファミリアプリケーションの名前。</span><span class="sxs-lookup"><span data-stu-id="5a66c-151">Windows Package Family Name of application.</span></span> |
|<span data-ttu-id="5a66c-152">appservicename</span><span class="sxs-lookup"><span data-stu-id="5a66c-152">appServiceName</span></span> | <span data-ttu-id="5a66c-153">String</span><span class="sxs-lookup"><span data-stu-id="5a66c-153">String</span></span> | <span data-ttu-id="5a66c-154">ターゲットアプリケーションによって定義された app service の名前です。</span><span class="sxs-lookup"><span data-stu-id="5a66c-154">Name of app service defined by the target application.</span></span> <span data-ttu-id="5a66c-155">app service を開始する場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="5a66c-155">Required if launching an app service.</span></span> |
|<span data-ttu-id="5a66c-156">type</span><span class="sxs-lookup"><span data-stu-id="5a66c-156">type</span></span>| <span data-ttu-id="5a66c-157">String</span><span class="sxs-lookup"><span data-stu-id="5a66c-157">String</span></span> | <span data-ttu-id="5a66c-158">launchuri または AppService。</span><span class="sxs-lookup"><span data-stu-id="5a66c-158">LaunchURI or AppService.</span></span> |
|<span data-ttu-id="5a66c-159">id</span><span class="sxs-lookup"><span data-stu-id="5a66c-159">id</span></span>| <span data-ttu-id="5a66c-160">String</span><span class="sxs-lookup"><span data-stu-id="5a66c-160">String</span></span> | <span data-ttu-id="5a66c-161">デバイスに送信されたコマンドの ID。</span><span class="sxs-lookup"><span data-stu-id="5a66c-161">The ID of a command that has been sent to the device.</span></span> |
|<span data-ttu-id="5a66c-162">actionstatus</span><span class="sxs-lookup"><span data-stu-id="5a66c-162">actionStatus</span></span> | <span data-ttu-id="5a66c-163">String</span><span class="sxs-lookup"><span data-stu-id="5a66c-163">String</span></span> | <span data-ttu-id="5a66c-164">コマンドの[状態](get-device-command-status.md)を示します。</span><span class="sxs-lookup"><span data-stu-id="5a66c-164">The [status](get-device-command-status.md) of a command.</span></span> |
|<span data-ttu-id="5a66c-165">error</span><span class="sxs-lookup"><span data-stu-id="5a66c-165">error</span></span>| <span data-ttu-id="5a66c-166">String</span><span class="sxs-lookup"><span data-stu-id="5a66c-166">String</span></span>| <span data-ttu-id="5a66c-167">ターゲットアプリケーションからの要求に関連付けられているエラー。</span><span class="sxs-lookup"><span data-stu-id="5a66c-167">Any errors associated with the request from the target application.</span></span> |

## <a name="launch-uri-example"></a><span data-ttu-id="5a66c-168">開始 URI の例</span><span class="sxs-lookup"><span data-stu-id="5a66c-168">Launch URI example</span></span>

<span data-ttu-id="5a66c-169">ここでは、launchuri 要求の例を示します。ターゲットデバイス上の URI またはアプリケーションを起動します。</span><span class="sxs-lookup"><span data-stu-id="5a66c-169">Here is an example of a LaunchURI request; it will launch a URI or an application on the target device.</span></span> <span data-ttu-id="5a66c-170">URI またはアプリを起動するには、デバイスの ID を使用して POST を発行します (GET 呼び出し`me/devices`の実行によって取得されます)。</span><span class="sxs-lookup"><span data-stu-id="5a66c-170">To launch a URI or an app, issue a POST using the ID of the device (obtained from doing a GET call on `me/devices`).</span></span> <span data-ttu-id="5a66c-171">*型*パラメーターを*launchuri*に設定し、などの URI 値をhttps://bing.com指定します。</span><span class="sxs-lookup"><span data-stu-id="5a66c-171">Set the *Type* parameters to *LaunchURI* and provide a URI value such as https://bing.com.</span></span>

#### <a name="request"></a><span data-ttu-id="5a66c-172">要求</span><span class="sxs-lookup"><span data-stu-id="5a66c-172">Request</span></span>

<span data-ttu-id="5a66c-173">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5a66c-173">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="5a66c-174">応答</span><span class="sxs-lookup"><span data-stu-id="5a66c-174">Response</span></span> 

<span data-ttu-id="5a66c-175">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5a66c-175">The following is an example of the response.</span></span>

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


## <a name="app-service-example"></a><span data-ttu-id="5a66c-176">App service の例</span><span class="sxs-lookup"><span data-stu-id="5a66c-176">App service example</span></span>

<span data-ttu-id="5a66c-177">ここでは、デバイス上の app service に対してクエリを実行する例を示します。</span><span class="sxs-lookup"><span data-stu-id="5a66c-177">Here is an example of querying an app service on a device.</span></span> <span data-ttu-id="5a66c-178">アプリサービスを使用するには、デバイスの id を使用して POST 呼び出しを行う必要があります (GET `me/devices`呼び出しの実行によって取得)。</span><span class="sxs-lookup"><span data-stu-id="5a66c-178">To use an app service you must do a POST call using the id of the device (obtained from doing a GET call on `me/devices`).</span></span> <span data-ttu-id="5a66c-179">次の例を使用するには、ターゲットデバイスに[ローマアプリ](https://aka.ms/romanapp)をインストールする必要があります。</span><span class="sxs-lookup"><span data-stu-id="5a66c-179">To use the following example, you must install the [Rome app](https://aka.ms/romanapp) on your target device.</span></span>

<span data-ttu-id="5a66c-180">呼び出しでは、いくつかの追加プロパティを設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="5a66c-180">Several additional properties must be set in the call.</span></span> <span data-ttu-id="5a66c-181">*Type*を*AppService*に設定する必要があります。 *appservicename*は、アプリケーションで定義されている app service \*\* の名前に設定する必要があります。また、アプリマニフェストで定義されているパッケージファミリー名と*ペイロード*に設定する必要があります。ターゲットアプリケーション内で呼び出すサービスのキーと値を保持します。</span><span class="sxs-lookup"><span data-stu-id="5a66c-181">*Type* must be set to *AppService*, *AppServiceName* must be set to the name of the app service defined in the application, *PackageFamilyName* must be set to the package family name defined in the app manifest, and *Payload* holds the keys and values for the service you are calling within the target application.</span></span>

#### <a name="request"></a><span data-ttu-id="5a66c-182">要求</span><span class="sxs-lookup"><span data-stu-id="5a66c-182">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="5a66c-183">応答</span><span class="sxs-lookup"><span data-stu-id="5a66c-183">Response</span></span>

<span data-ttu-id="5a66c-184">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5a66c-184">The following is an example of the response.</span></span>

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
