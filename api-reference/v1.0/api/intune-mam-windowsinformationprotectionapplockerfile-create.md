---
title: windowsInformationProtectionAppLockerFile の作成
description: 新しい windowsInformationProtectionAppLockerFile オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a7b6bfb8271e6b462be1d18fd509da33aea836b3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967596"
---
# <a name="create-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="46e8e-103">windowsInformationProtectionAppLockerFile の作成</span><span class="sxs-lookup"><span data-stu-id="46e8e-103">Create windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="46e8e-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="46e8e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="46e8e-105">新しい [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="46e8e-105">Create a new [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="46e8e-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="46e8e-106">Prerequisites</span></span>
<span data-ttu-id="46e8e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="46e8e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46e8e-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="46e8e-109">Permission type</span></span>|<span data-ttu-id="46e8e-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="46e8e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46e8e-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="46e8e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="46e8e-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46e8e-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="46e8e-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="46e8e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46e8e-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="46e8e-114">Not supported.</span></span>|
|<span data-ttu-id="46e8e-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="46e8e-115">Application</span></span>|<span data-ttu-id="46e8e-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="46e8e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="46e8e-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="46e8e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles
POST /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/protectedAppLockerFiles
POST /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/exemptAppLockerFiles
POST /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/protectedAppLockerFiles
```

## <a name="request-headers"></a><span data-ttu-id="46e8e-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="46e8e-118">Request headers</span></span>
|<span data-ttu-id="46e8e-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="46e8e-119">Header</span></span>|<span data-ttu-id="46e8e-120">値</span><span class="sxs-lookup"><span data-stu-id="46e8e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46e8e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="46e8e-121">Authorization</span></span>|<span data-ttu-id="46e8e-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="46e8e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46e8e-123">Accept</span><span class="sxs-lookup"><span data-stu-id="46e8e-123">Accept</span></span>|<span data-ttu-id="46e8e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="46e8e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46e8e-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="46e8e-125">Request body</span></span>
<span data-ttu-id="46e8e-126">要求本文で、windowsInformationProtectionAppLockerFile オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="46e8e-126">In the request body, supply a JSON representation for the windowsInformationProtectionAppLockerFile object.</span></span>

<span data-ttu-id="46e8e-127">次の表に、windowsInformationProtectionAppLockerFile の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="46e8e-127">The following table shows the properties that are required when you create the windowsInformationProtectionAppLockerFile.</span></span>

|<span data-ttu-id="46e8e-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="46e8e-128">Property</span></span>|<span data-ttu-id="46e8e-129">種類</span><span class="sxs-lookup"><span data-stu-id="46e8e-129">Type</span></span>|<span data-ttu-id="46e8e-130">説明</span><span class="sxs-lookup"><span data-stu-id="46e8e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46e8e-131">displayName</span><span class="sxs-lookup"><span data-stu-id="46e8e-131">displayName</span></span>|<span data-ttu-id="46e8e-132">String</span><span class="sxs-lookup"><span data-stu-id="46e8e-132">String</span></span>|<span data-ttu-id="46e8e-133">フレンドリ名</span><span class="sxs-lookup"><span data-stu-id="46e8e-133">The friendly name</span></span>|
|<span data-ttu-id="46e8e-134">fileHash</span><span class="sxs-lookup"><span data-stu-id="46e8e-134">fileHash</span></span>|<span data-ttu-id="46e8e-135">String</span><span class="sxs-lookup"><span data-stu-id="46e8e-135">String</span></span>|<span data-ttu-id="46e8e-136">ファイルの SHA256 ハッシュ</span><span class="sxs-lookup"><span data-stu-id="46e8e-136">SHA256 hash of the file</span></span>|
|<span data-ttu-id="46e8e-137">file</span><span class="sxs-lookup"><span data-stu-id="46e8e-137">file</span></span>|<span data-ttu-id="46e8e-138">Binary</span><span class="sxs-lookup"><span data-stu-id="46e8e-138">Binary</span></span>|<span data-ttu-id="46e8e-139">バイト配列のファイル</span><span class="sxs-lookup"><span data-stu-id="46e8e-139">File as a byte array</span></span>|
|<span data-ttu-id="46e8e-140">id</span><span class="sxs-lookup"><span data-stu-id="46e8e-140">id</span></span>|<span data-ttu-id="46e8e-141">String</span><span class="sxs-lookup"><span data-stu-id="46e8e-141">String</span></span>|<span data-ttu-id="46e8e-142">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="46e8e-142">Key of the entity.</span></span>|
|<span data-ttu-id="46e8e-143">version</span><span class="sxs-lookup"><span data-stu-id="46e8e-143">version</span></span>|<span data-ttu-id="46e8e-144">String</span><span class="sxs-lookup"><span data-stu-id="46e8e-144">String</span></span>|<span data-ttu-id="46e8e-145">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="46e8e-145">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="46e8e-146">応答</span><span class="sxs-lookup"><span data-stu-id="46e8e-146">Response</span></span>
<span data-ttu-id="46e8e-147">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="46e8e-147">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46e8e-148">例</span><span class="sxs-lookup"><span data-stu-id="46e8e-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="46e8e-149">要求</span><span class="sxs-lookup"><span data-stu-id="46e8e-149">Request</span></span>
<span data-ttu-id="46e8e-150">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="46e8e-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles
Content-type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLockerFile",
  "displayName": "Display Name value",
  "fileHash": "File Hash value",
  "file": "ZmlsZQ==",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="46e8e-151">応答</span><span class="sxs-lookup"><span data-stu-id="46e8e-151">Response</span></span>
<span data-ttu-id="46e8e-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="46e8e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 260

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLockerFile",
  "displayName": "Display Name value",
  "fileHash": "File Hash value",
  "file": "ZmlsZQ==",
  "id": "d81f0e40-0e40-d81f-400e-1fd8400e1fd8",
  "version": "Version value"
}
```



