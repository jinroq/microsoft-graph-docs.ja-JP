---
title: windowsInformationProtectionAppLockerFile の更新
description: windowsInformationProtectionAppLockerFile オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 97afdcc7a7d0f0025b19ed33e9df2e10e9b275fa
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32453596"
---
# <a name="update-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="41a8b-103">windowsInformationProtectionAppLockerFile の更新</span><span class="sxs-lookup"><span data-stu-id="41a8b-103">Update windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="41a8b-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="41a8b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41a8b-105">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="41a8b-105">Update the properties of a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="41a8b-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="41a8b-106">Prerequisites</span></span>
<span data-ttu-id="41a8b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="41a8b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41a8b-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="41a8b-109">Permission type</span></span>|<span data-ttu-id="41a8b-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="41a8b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41a8b-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="41a8b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="41a8b-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41a8b-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="41a8b-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="41a8b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41a8b-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="41a8b-114">Not supported.</span></span>|
|<span data-ttu-id="41a8b-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="41a8b-115">Application</span></span>|<span data-ttu-id="41a8b-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="41a8b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="41a8b-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="41a8b-117">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="41a8b-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="41a8b-118">Request headers</span></span>
|<span data-ttu-id="41a8b-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="41a8b-119">Header</span></span>|<span data-ttu-id="41a8b-120">値</span><span class="sxs-lookup"><span data-stu-id="41a8b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="41a8b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="41a8b-121">Authorization</span></span>|<span data-ttu-id="41a8b-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="41a8b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="41a8b-123">承諾</span><span class="sxs-lookup"><span data-stu-id="41a8b-123">Accept</span></span>|<span data-ttu-id="41a8b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="41a8b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41a8b-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="41a8b-125">Request body</span></span>
<span data-ttu-id="41a8b-126">要求本文で、[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="41a8b-126">In the request body, supply a JSON representation for the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

<span data-ttu-id="41a8b-127">次の表に、[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="41a8b-127">The following table shows the properties that are required when you create the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span></span>

|<span data-ttu-id="41a8b-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="41a8b-128">Property</span></span>|<span data-ttu-id="41a8b-129">型</span><span class="sxs-lookup"><span data-stu-id="41a8b-129">Type</span></span>|<span data-ttu-id="41a8b-130">説明</span><span class="sxs-lookup"><span data-stu-id="41a8b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41a8b-131">displayName</span><span class="sxs-lookup"><span data-stu-id="41a8b-131">displayName</span></span>|<span data-ttu-id="41a8b-132">String</span><span class="sxs-lookup"><span data-stu-id="41a8b-132">String</span></span>|<span data-ttu-id="41a8b-133">フレンドリ名</span><span class="sxs-lookup"><span data-stu-id="41a8b-133">The friendly name</span></span>|
|<span data-ttu-id="41a8b-134">fileHash</span><span class="sxs-lookup"><span data-stu-id="41a8b-134">fileHash</span></span>|<span data-ttu-id="41a8b-135">String</span><span class="sxs-lookup"><span data-stu-id="41a8b-135">String</span></span>|<span data-ttu-id="41a8b-136">ファイルの SHA256 ハッシュ</span><span class="sxs-lookup"><span data-stu-id="41a8b-136">SHA256 hash of the file</span></span>|
|<span data-ttu-id="41a8b-137">file</span><span class="sxs-lookup"><span data-stu-id="41a8b-137">file</span></span>|<span data-ttu-id="41a8b-138">Binary</span><span class="sxs-lookup"><span data-stu-id="41a8b-138">Binary</span></span>|<span data-ttu-id="41a8b-139">バイト配列のファイル</span><span class="sxs-lookup"><span data-stu-id="41a8b-139">File as a byte array</span></span>|
|<span data-ttu-id="41a8b-140">id</span><span class="sxs-lookup"><span data-stu-id="41a8b-140">id</span></span>|<span data-ttu-id="41a8b-141">String</span><span class="sxs-lookup"><span data-stu-id="41a8b-141">String</span></span>|<span data-ttu-id="41a8b-142">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="41a8b-142">Key of the entity.</span></span>|
|<span data-ttu-id="41a8b-143">version</span><span class="sxs-lookup"><span data-stu-id="41a8b-143">version</span></span>|<span data-ttu-id="41a8b-144">String</span><span class="sxs-lookup"><span data-stu-id="41a8b-144">String</span></span>|<span data-ttu-id="41a8b-145">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="41a8b-145">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="41a8b-146">応答</span><span class="sxs-lookup"><span data-stu-id="41a8b-146">Response</span></span>
<span data-ttu-id="41a8b-147">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="41a8b-147">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41a8b-148">例</span><span class="sxs-lookup"><span data-stu-id="41a8b-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="41a8b-149">要求</span><span class="sxs-lookup"><span data-stu-id="41a8b-149">Request</span></span>
<span data-ttu-id="41a8b-150">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="41a8b-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="41a8b-151">応答</span><span class="sxs-lookup"><span data-stu-id="41a8b-151">Response</span></span>
<span data-ttu-id="41a8b-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="41a8b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



