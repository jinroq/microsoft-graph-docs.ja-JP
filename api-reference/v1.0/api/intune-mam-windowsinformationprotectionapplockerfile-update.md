---
title: windowsInformationProtectionAppLockerFile の更新
description: windowsInformationProtectionAppLockerFile オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6e6d81b953288e1c8c9435a9502616f3f9fbc1d4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923825"
---
# <a name="update-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="e3e55-103">windowsInformationProtectionAppLockerFile の更新</span><span class="sxs-lookup"><span data-stu-id="e3e55-103">Update windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="e3e55-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e3e55-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e3e55-105">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e3e55-105">Update the properties of a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e3e55-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="e3e55-106">Prerequisites</span></span>
<span data-ttu-id="e3e55-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e3e55-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3e55-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e3e55-109">Permission type</span></span>|<span data-ttu-id="e3e55-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e3e55-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e3e55-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e3e55-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e3e55-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3e55-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e3e55-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e3e55-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3e55-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e3e55-114">Not supported.</span></span>|
|<span data-ttu-id="e3e55-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e3e55-115">Application</span></span>|<span data-ttu-id="e3e55-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e3e55-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e3e55-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e3e55-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
PATCH /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/protectedAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
PATCH /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
PATCH /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/protectedAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
```

## <a name="request-headers"></a><span data-ttu-id="e3e55-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e3e55-118">Request headers</span></span>
|<span data-ttu-id="e3e55-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e3e55-119">Header</span></span>|<span data-ttu-id="e3e55-120">値</span><span class="sxs-lookup"><span data-stu-id="e3e55-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e3e55-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3e55-121">Authorization</span></span>|<span data-ttu-id="e3e55-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="e3e55-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e3e55-123">Accept</span><span class="sxs-lookup"><span data-stu-id="e3e55-123">Accept</span></span>|<span data-ttu-id="e3e55-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e3e55-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3e55-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="e3e55-125">Request body</span></span>
<span data-ttu-id="e3e55-126">要求本文で、[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e3e55-126">In the request body, supply a JSON representation for the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

<span data-ttu-id="e3e55-127">次の表に、[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="e3e55-127">The following table shows the properties that are required when you create the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span></span>

|<span data-ttu-id="e3e55-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e3e55-128">Property</span></span>|<span data-ttu-id="e3e55-129">種類</span><span class="sxs-lookup"><span data-stu-id="e3e55-129">Type</span></span>|<span data-ttu-id="e3e55-130">説明</span><span class="sxs-lookup"><span data-stu-id="e3e55-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3e55-131">displayName</span><span class="sxs-lookup"><span data-stu-id="e3e55-131">displayName</span></span>|<span data-ttu-id="e3e55-132">String</span><span class="sxs-lookup"><span data-stu-id="e3e55-132">String</span></span>|<span data-ttu-id="e3e55-133">フレンドリ名</span><span class="sxs-lookup"><span data-stu-id="e3e55-133">The friendly name</span></span>|
|<span data-ttu-id="e3e55-134">fileHash</span><span class="sxs-lookup"><span data-stu-id="e3e55-134">fileHash</span></span>|<span data-ttu-id="e3e55-135">String</span><span class="sxs-lookup"><span data-stu-id="e3e55-135">String</span></span>|<span data-ttu-id="e3e55-136">ファイルの SHA256 ハッシュ</span><span class="sxs-lookup"><span data-stu-id="e3e55-136">SHA256 hash of the file</span></span>|
|<span data-ttu-id="e3e55-137">file</span><span class="sxs-lookup"><span data-stu-id="e3e55-137">file</span></span>|<span data-ttu-id="e3e55-138">Binary</span><span class="sxs-lookup"><span data-stu-id="e3e55-138">Binary</span></span>|<span data-ttu-id="e3e55-139">バイト配列のファイル</span><span class="sxs-lookup"><span data-stu-id="e3e55-139">File as a byte array</span></span>|
|<span data-ttu-id="e3e55-140">id</span><span class="sxs-lookup"><span data-stu-id="e3e55-140">id</span></span>|<span data-ttu-id="e3e55-141">String</span><span class="sxs-lookup"><span data-stu-id="e3e55-141">String</span></span>|<span data-ttu-id="e3e55-142">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e3e55-142">Key of the entity.</span></span>|
|<span data-ttu-id="e3e55-143">version</span><span class="sxs-lookup"><span data-stu-id="e3e55-143">version</span></span>|<span data-ttu-id="e3e55-144">String</span><span class="sxs-lookup"><span data-stu-id="e3e55-144">String</span></span>|<span data-ttu-id="e3e55-145">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="e3e55-145">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="e3e55-146">応答</span><span class="sxs-lookup"><span data-stu-id="e3e55-146">Response</span></span>
<span data-ttu-id="e3e55-147">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e3e55-147">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3e55-148">例</span><span class="sxs-lookup"><span data-stu-id="e3e55-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="e3e55-149">要求</span><span class="sxs-lookup"><span data-stu-id="e3e55-149">Request</span></span>
<span data-ttu-id="e3e55-150">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e3e55-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
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

### <a name="response"></a><span data-ttu-id="e3e55-151">応答</span><span class="sxs-lookup"><span data-stu-id="e3e55-151">Response</span></span>
<span data-ttu-id="e3e55-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e3e55-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



