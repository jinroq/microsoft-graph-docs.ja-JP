---
title: windowsInformationProtectionAppLockerFile の作成
description: 新しい windowsInformationProtectionAppLockerFile オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d22e4be6d282ba7750b6c896b2592ea8b0b71a62
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30984038"
---
# <a name="create-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="46da1-103">windowsInformationProtectionAppLockerFile の作成</span><span class="sxs-lookup"><span data-stu-id="46da1-103">Create windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="46da1-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="46da1-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46da1-105">新しい [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="46da1-105">Create a new [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="46da1-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="46da1-106">Prerequisites</span></span>
<span data-ttu-id="46da1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="46da1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46da1-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="46da1-109">Permission type</span></span>|<span data-ttu-id="46da1-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="46da1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46da1-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="46da1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="46da1-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46da1-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="46da1-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="46da1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46da1-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="46da1-114">Not supported.</span></span>|
|<span data-ttu-id="46da1-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="46da1-115">Application</span></span>|<span data-ttu-id="46da1-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="46da1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="46da1-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="46da1-117">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="46da1-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="46da1-118">Request headers</span></span>
|<span data-ttu-id="46da1-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="46da1-119">Header</span></span>|<span data-ttu-id="46da1-120">値</span><span class="sxs-lookup"><span data-stu-id="46da1-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46da1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="46da1-121">Authorization</span></span>|<span data-ttu-id="46da1-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="46da1-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46da1-123">承諾</span><span class="sxs-lookup"><span data-stu-id="46da1-123">Accept</span></span>|<span data-ttu-id="46da1-124">application/json</span><span class="sxs-lookup"><span data-stu-id="46da1-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46da1-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="46da1-125">Request body</span></span>
<span data-ttu-id="46da1-126">要求本文で、windowsInformationProtectionAppLockerFile オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="46da1-126">In the request body, supply a JSON representation for the windowsInformationProtectionAppLockerFile object.</span></span>

<span data-ttu-id="46da1-127">次の表に、windowsInformationProtectionAppLockerFile の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="46da1-127">The following table shows the properties that are required when you create the windowsInformationProtectionAppLockerFile.</span></span>

|<span data-ttu-id="46da1-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="46da1-128">Property</span></span>|<span data-ttu-id="46da1-129">型</span><span class="sxs-lookup"><span data-stu-id="46da1-129">Type</span></span>|<span data-ttu-id="46da1-130">説明</span><span class="sxs-lookup"><span data-stu-id="46da1-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46da1-131">displayName</span><span class="sxs-lookup"><span data-stu-id="46da1-131">displayName</span></span>|<span data-ttu-id="46da1-132">String</span><span class="sxs-lookup"><span data-stu-id="46da1-132">String</span></span>|<span data-ttu-id="46da1-133">フレンドリ名</span><span class="sxs-lookup"><span data-stu-id="46da1-133">The friendly name</span></span>|
|<span data-ttu-id="46da1-134">fileHash</span><span class="sxs-lookup"><span data-stu-id="46da1-134">fileHash</span></span>|<span data-ttu-id="46da1-135">String</span><span class="sxs-lookup"><span data-stu-id="46da1-135">String</span></span>|<span data-ttu-id="46da1-136">ファイルの SHA256 ハッシュ</span><span class="sxs-lookup"><span data-stu-id="46da1-136">SHA256 hash of the file</span></span>|
|<span data-ttu-id="46da1-137">file</span><span class="sxs-lookup"><span data-stu-id="46da1-137">file</span></span>|<span data-ttu-id="46da1-138">Binary</span><span class="sxs-lookup"><span data-stu-id="46da1-138">Binary</span></span>|<span data-ttu-id="46da1-139">バイト配列のファイル</span><span class="sxs-lookup"><span data-stu-id="46da1-139">File as a byte array</span></span>|
|<span data-ttu-id="46da1-140">id</span><span class="sxs-lookup"><span data-stu-id="46da1-140">id</span></span>|<span data-ttu-id="46da1-141">String</span><span class="sxs-lookup"><span data-stu-id="46da1-141">String</span></span>|<span data-ttu-id="46da1-142">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="46da1-142">Key of the entity.</span></span>|
|<span data-ttu-id="46da1-143">version</span><span class="sxs-lookup"><span data-stu-id="46da1-143">version</span></span>|<span data-ttu-id="46da1-144">String</span><span class="sxs-lookup"><span data-stu-id="46da1-144">String</span></span>|<span data-ttu-id="46da1-145">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="46da1-145">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="46da1-146">応答</span><span class="sxs-lookup"><span data-stu-id="46da1-146">Response</span></span>
<span data-ttu-id="46da1-147">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="46da1-147">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46da1-148">例</span><span class="sxs-lookup"><span data-stu-id="46da1-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="46da1-149">要求</span><span class="sxs-lookup"><span data-stu-id="46da1-149">Request</span></span>
<span data-ttu-id="46da1-150">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="46da1-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="46da1-151">応答</span><span class="sxs-lookup"><span data-stu-id="46da1-151">Response</span></span>
<span data-ttu-id="46da1-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="46da1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



