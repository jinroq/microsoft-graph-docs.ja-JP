---
title: DeviceManagementScript を更新します。
description: DeviceManagementScript オブジェクトのプロパティを更新します。
ms.openlocfilehash: d88579f130607b08b0d34620b701be5c239bc03f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069614"
---
# <a name="update-devicemanagementscript"></a><span data-ttu-id="5fc57-103">DeviceManagementScript を更新します。</span><span class="sxs-lookup"><span data-stu-id="5fc57-103">Update deviceManagementScript</span></span>

> <span data-ttu-id="5fc57-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5fc57-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5fc57-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5fc57-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5fc57-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5fc57-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5fc57-107">[DeviceManagementScript](../resources/intune-devices-devicemanagementscript.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="5fc57-107">Update the properties of a [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5fc57-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="5fc57-108">Prerequisites</span></span>
<span data-ttu-id="5fc57-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5fc57-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5fc57-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5fc57-111">Permission type</span></span>|<span data-ttu-id="5fc57-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="5fc57-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5fc57-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5fc57-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5fc57-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5fc57-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="5fc57-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5fc57-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5fc57-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5fc57-116">Not supported.</span></span>|
|<span data-ttu-id="5fc57-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5fc57-117">Application</span></span>|<span data-ttu-id="5fc57-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5fc57-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5fc57-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5fc57-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="5fc57-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5fc57-120">Request headers</span></span>
|<span data-ttu-id="5fc57-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5fc57-121">Header</span></span>|<span data-ttu-id="5fc57-122">値</span><span class="sxs-lookup"><span data-stu-id="5fc57-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5fc57-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5fc57-123">Authorization</span></span>|<span data-ttu-id="5fc57-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="5fc57-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5fc57-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5fc57-125">Accept</span></span>|<span data-ttu-id="5fc57-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5fc57-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5fc57-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="5fc57-127">Request body</span></span>
<span data-ttu-id="5fc57-128">要求の本文に[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="5fc57-128">In the request body, supply a JSON representation for the [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object.</span></span>

<span data-ttu-id="5fc57-129">[DeviceManagementScript](../resources/intune-devices-devicemanagementscript.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="5fc57-129">The following table shows the properties that are required when you create the [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md).</span></span>

|<span data-ttu-id="5fc57-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5fc57-130">Property</span></span>|<span data-ttu-id="5fc57-131">型</span><span class="sxs-lookup"><span data-stu-id="5fc57-131">Type</span></span>|<span data-ttu-id="5fc57-132">説明</span><span class="sxs-lookup"><span data-stu-id="5fc57-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5fc57-133">id</span><span class="sxs-lookup"><span data-stu-id="5fc57-133">id</span></span>|<span data-ttu-id="5fc57-134">String</span><span class="sxs-lookup"><span data-stu-id="5fc57-134">String</span></span>|<span data-ttu-id="5fc57-135">デバイス管理スクリプト用の一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="5fc57-135">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="5fc57-136">displayName</span><span class="sxs-lookup"><span data-stu-id="5fc57-136">displayName</span></span>|<span data-ttu-id="5fc57-137">String</span><span class="sxs-lookup"><span data-stu-id="5fc57-137">String</span></span>|<span data-ttu-id="5fc57-138">デバイスの管理スクリプトの名前です。</span><span class="sxs-lookup"><span data-stu-id="5fc57-138">Name of the device management script.</span></span>|
|<span data-ttu-id="5fc57-139">説明</span><span class="sxs-lookup"><span data-stu-id="5fc57-139">description</span></span>|<span data-ttu-id="5fc57-140">String</span><span class="sxs-lookup"><span data-stu-id="5fc57-140">String</span></span>|<span data-ttu-id="5fc57-141">デバイスの管理スクリプトのオプションの説明です。</span><span class="sxs-lookup"><span data-stu-id="5fc57-141">Optional description for the device management script.</span></span>|
|<span data-ttu-id="5fc57-142">runSchedule</span><span class="sxs-lookup"><span data-stu-id="5fc57-142">runSchedule</span></span>|[<span data-ttu-id="5fc57-143">runSchedule</span><span class="sxs-lookup"><span data-stu-id="5fc57-143">runSchedule</span></span>](../resources/intune-devices-runschedule.md)|<span data-ttu-id="5fc57-144">スクリプトを実行する間隔です。</span><span class="sxs-lookup"><span data-stu-id="5fc57-144">The interval for script to run.</span></span> <span data-ttu-id="5fc57-145">定義されていないスクリプトは実行 1 回</span><span class="sxs-lookup"><span data-stu-id="5fc57-145">If not defined the script will run once</span></span>|
|<span data-ttu-id="5fc57-146">scriptContent</span><span class="sxs-lookup"><span data-stu-id="5fc57-146">scriptContent</span></span>|<span data-ttu-id="5fc57-147">バイナリ</span><span class="sxs-lookup"><span data-stu-id="5fc57-147">Binary</span></span>|<span data-ttu-id="5fc57-148">スクリプトの内容。</span><span class="sxs-lookup"><span data-stu-id="5fc57-148">The script content.</span></span>|
|<span data-ttu-id="5fc57-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5fc57-149">createdDateTime</span></span>|<span data-ttu-id="5fc57-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5fc57-150">DateTimeOffset</span></span>|<span data-ttu-id="5fc57-151">デバイス管理スクリプトが作成された日時です。</span><span class="sxs-lookup"><span data-stu-id="5fc57-151">The date and time the device management script was created.</span></span>|
|<span data-ttu-id="5fc57-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5fc57-152">lastModifiedDateTime</span></span>|<span data-ttu-id="5fc57-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5fc57-153">DateTimeOffset</span></span>|<span data-ttu-id="5fc57-154">日付と時刻、デバイス管理のスクリプトが最後に修正されました。</span><span class="sxs-lookup"><span data-stu-id="5fc57-154">The date and time the device management script was last modified.</span></span>|
|<span data-ttu-id="5fc57-155">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="5fc57-155">runAsAccount</span></span>|[<span data-ttu-id="5fc57-156">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="5fc57-156">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="5fc57-157">デバイス管理のスクリプトで実行される実行コンテキストの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="5fc57-157">Indicates the type of execution context the device management script runs in.</span></span> <span data-ttu-id="5fc57-158">使用可能な値は、`system`、`user` です。</span><span class="sxs-lookup"><span data-stu-id="5fc57-158">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="5fc57-159">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="5fc57-159">enforceSignatureCheck</span></span>|<span data-ttu-id="5fc57-160">ブール値</span><span class="sxs-lookup"><span data-stu-id="5fc57-160">Boolean</span></span>|<span data-ttu-id="5fc57-161">スクリプト署名をチェックする必要があるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="5fc57-161">Indicate whether the script signature needs be checked.</span></span>|
|<span data-ttu-id="5fc57-162">fileName</span><span class="sxs-lookup"><span data-stu-id="5fc57-162">fileName</span></span>|<span data-ttu-id="5fc57-163">String</span><span class="sxs-lookup"><span data-stu-id="5fc57-163">String</span></span>|<span data-ttu-id="5fc57-164">スクリプト ファイルの名前です。</span><span class="sxs-lookup"><span data-stu-id="5fc57-164">Script file name.</span></span>|



## <a name="response"></a><span data-ttu-id="5fc57-165">応答</span><span class="sxs-lookup"><span data-stu-id="5fc57-165">Response</span></span>
<span data-ttu-id="5fc57-166">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="5fc57-166">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5fc57-167">例</span><span class="sxs-lookup"><span data-stu-id="5fc57-167">Example</span></span>
### <a name="request"></a><span data-ttu-id="5fc57-168">要求</span><span class="sxs-lookup"><span data-stu-id="5fc57-168">Request</span></span>
<span data-ttu-id="5fc57-169">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5fc57-169">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
Content-type: application/json
Content-length: 361

{
  "displayName": "Display Name value",
  "description": "Description value",
  "runSchedule": {
    "@odata.type": "microsoft.graph.runSchedule"
  },
  "scriptContent": "c2NyaXB0Q29udGVudA==",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "runAsAccount": "user",
  "enforceSignatureCheck": true,
  "fileName": "File Name value"
}
```

### <a name="response"></a><span data-ttu-id="5fc57-170">応答</span><span class="sxs-lookup"><span data-stu-id="5fc57-170">Response</span></span>
<span data-ttu-id="5fc57-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5fc57-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 530

{
  "@odata.type": "#microsoft.graph.deviceManagementScript",
  "id": "59ea4525-4525-59ea-2545-ea592545ea59",
  "displayName": "Display Name value",
  "description": "Description value",
  "runSchedule": {
    "@odata.type": "microsoft.graph.runSchedule"
  },
  "scriptContent": "c2NyaXB0Q29udGVudA==",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "runAsAccount": "user",
  "enforceSignatureCheck": true,
  "fileName": "File Name value"
}
```




