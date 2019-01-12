---
title: DeviceManagementScript を作成します。
description: 新しい deviceManagementScript オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3ef3f9436de79b5839912a44915238267f0c26dd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924028"
---
# <a name="create-devicemanagementscript"></a><span data-ttu-id="fb33a-103">DeviceManagementScript を作成します。</span><span class="sxs-lookup"><span data-stu-id="fb33a-103">Create deviceManagementScript</span></span>

> <span data-ttu-id="fb33a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fb33a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fb33a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fb33a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fb33a-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="fb33a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fb33a-107">新しい[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="fb33a-107">Create a new [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fb33a-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="fb33a-108">Prerequisites</span></span>
<span data-ttu-id="fb33a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fb33a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb33a-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fb33a-111">Permission type</span></span>|<span data-ttu-id="fb33a-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="fb33a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb33a-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fb33a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fb33a-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb33a-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="fb33a-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fb33a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb33a-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fb33a-116">Not supported.</span></span>|
|<span data-ttu-id="fb33a-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fb33a-117">Application</span></span>|<span data-ttu-id="fb33a-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fb33a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb33a-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fb33a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts
```

## <a name="request-headers"></a><span data-ttu-id="fb33a-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fb33a-120">Request headers</span></span>
|<span data-ttu-id="fb33a-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fb33a-121">Header</span></span>|<span data-ttu-id="fb33a-122">値</span><span class="sxs-lookup"><span data-stu-id="fb33a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb33a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fb33a-123">Authorization</span></span>|<span data-ttu-id="fb33a-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="fb33a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fb33a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fb33a-125">Accept</span></span>|<span data-ttu-id="fb33a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fb33a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb33a-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="fb33a-127">Request body</span></span>
<span data-ttu-id="fb33a-128">要求の本文に deviceManagementScript オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="fb33a-128">In the request body, supply a JSON representation for the deviceManagementScript object.</span></span>

<span data-ttu-id="fb33a-129">次の表は、deviceManagementScript を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="fb33a-129">The following table shows the properties that are required when you create the deviceManagementScript.</span></span>

|<span data-ttu-id="fb33a-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fb33a-130">Property</span></span>|<span data-ttu-id="fb33a-131">型</span><span class="sxs-lookup"><span data-stu-id="fb33a-131">Type</span></span>|<span data-ttu-id="fb33a-132">説明</span><span class="sxs-lookup"><span data-stu-id="fb33a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb33a-133">ID</span><span class="sxs-lookup"><span data-stu-id="fb33a-133">id</span></span>|<span data-ttu-id="fb33a-134">String</span><span class="sxs-lookup"><span data-stu-id="fb33a-134">String</span></span>|<span data-ttu-id="fb33a-135">デバイス管理スクリプト用の一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="fb33a-135">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="fb33a-136">displayName</span><span class="sxs-lookup"><span data-stu-id="fb33a-136">displayName</span></span>|<span data-ttu-id="fb33a-137">String</span><span class="sxs-lookup"><span data-stu-id="fb33a-137">String</span></span>|<span data-ttu-id="fb33a-138">デバイスの管理スクリプトの名前です。</span><span class="sxs-lookup"><span data-stu-id="fb33a-138">Name of the device management script.</span></span>|
|<span data-ttu-id="fb33a-139">説明</span><span class="sxs-lookup"><span data-stu-id="fb33a-139">description</span></span>|<span data-ttu-id="fb33a-140">String</span><span class="sxs-lookup"><span data-stu-id="fb33a-140">String</span></span>|<span data-ttu-id="fb33a-141">デバイスの管理スクリプトのオプションの説明です。</span><span class="sxs-lookup"><span data-stu-id="fb33a-141">Optional description for the device management script.</span></span>|
|<span data-ttu-id="fb33a-142">runSchedule</span><span class="sxs-lookup"><span data-stu-id="fb33a-142">runSchedule</span></span>|[<span data-ttu-id="fb33a-143">runSchedule</span><span class="sxs-lookup"><span data-stu-id="fb33a-143">runSchedule</span></span>](../resources/intune-devices-runschedule.md)|<span data-ttu-id="fb33a-144">スクリプトを実行する間隔です。</span><span class="sxs-lookup"><span data-stu-id="fb33a-144">The interval for script to run.</span></span> <span data-ttu-id="fb33a-145">定義されていないスクリプトは実行 1 回</span><span class="sxs-lookup"><span data-stu-id="fb33a-145">If not defined the script will run once</span></span>|
|<span data-ttu-id="fb33a-146">scriptContent</span><span class="sxs-lookup"><span data-stu-id="fb33a-146">scriptContent</span></span>|<span data-ttu-id="fb33a-147">Binary</span><span class="sxs-lookup"><span data-stu-id="fb33a-147">Binary</span></span>|<span data-ttu-id="fb33a-148">スクリプトの内容。</span><span class="sxs-lookup"><span data-stu-id="fb33a-148">The script content.</span></span>|
|<span data-ttu-id="fb33a-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fb33a-149">createdDateTime</span></span>|<span data-ttu-id="fb33a-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb33a-150">DateTimeOffset</span></span>|<span data-ttu-id="fb33a-151">デバイス管理スクリプトが作成された日時です。</span><span class="sxs-lookup"><span data-stu-id="fb33a-151">The date and time the device management script was created.</span></span>|
|<span data-ttu-id="fb33a-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fb33a-152">lastModifiedDateTime</span></span>|<span data-ttu-id="fb33a-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb33a-153">DateTimeOffset</span></span>|<span data-ttu-id="fb33a-154">日付と時刻、デバイス管理のスクリプトが最後に修正されました。</span><span class="sxs-lookup"><span data-stu-id="fb33a-154">The date and time the device management script was last modified.</span></span>|
|<span data-ttu-id="fb33a-155">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="fb33a-155">runAsAccount</span></span>|[<span data-ttu-id="fb33a-156">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="fb33a-156">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="fb33a-157">デバイス管理のスクリプトで実行される実行コンテキストの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="fb33a-157">Indicates the type of execution context the device management script runs in.</span></span> <span data-ttu-id="fb33a-158">使用可能な値は、`system`、`user` です。</span><span class="sxs-lookup"><span data-stu-id="fb33a-158">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="fb33a-159">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="fb33a-159">enforceSignatureCheck</span></span>|<span data-ttu-id="fb33a-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb33a-160">Boolean</span></span>|<span data-ttu-id="fb33a-161">スクリプト署名をチェックする必要があるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="fb33a-161">Indicate whether the script signature needs be checked.</span></span>|
|<span data-ttu-id="fb33a-162">fileName</span><span class="sxs-lookup"><span data-stu-id="fb33a-162">fileName</span></span>|<span data-ttu-id="fb33a-163">String</span><span class="sxs-lookup"><span data-stu-id="fb33a-163">String</span></span>|<span data-ttu-id="fb33a-164">スクリプト ファイルの名前です。</span><span class="sxs-lookup"><span data-stu-id="fb33a-164">Script file name.</span></span>|



## <a name="response"></a><span data-ttu-id="fb33a-165">応答</span><span class="sxs-lookup"><span data-stu-id="fb33a-165">Response</span></span>
<span data-ttu-id="fb33a-166">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="fb33a-166">If successful, this method returns a `201 Created` response code and a [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb33a-167">例</span><span class="sxs-lookup"><span data-stu-id="fb33a-167">Example</span></span>
### <a name="request"></a><span data-ttu-id="fb33a-168">要求</span><span class="sxs-lookup"><span data-stu-id="fb33a-168">Request</span></span>
<span data-ttu-id="fb33a-169">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fb33a-169">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts
Content-type: application/json
Content-length: 422

{
  "@odata.type": "#microsoft.graph.deviceManagementScript",
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

### <a name="response"></a><span data-ttu-id="fb33a-170">応答</span><span class="sxs-lookup"><span data-stu-id="fb33a-170">Response</span></span>
<span data-ttu-id="fb33a-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fb33a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





