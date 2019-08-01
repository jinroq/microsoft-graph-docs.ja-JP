---
title: windowsInformationProtectionAppLockerFile の作成
description: 新しい windowsInformationProtectionAppLockerFile オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 838731a8a55cf997efc42d43c14119c05e5d2b4b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35996582"
---
# <a name="create-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="1dc00-103">windowsInformationProtectionAppLockerFile の作成</span><span class="sxs-lookup"><span data-stu-id="1dc00-103">Create windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="1dc00-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1dc00-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1dc00-105">新しい [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="1dc00-105">Create a new [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1dc00-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="1dc00-106">Prerequisites</span></span>
<span data-ttu-id="1dc00-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1dc00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1dc00-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1dc00-109">Permission type</span></span>|<span data-ttu-id="1dc00-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1dc00-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1dc00-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1dc00-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1dc00-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1dc00-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1dc00-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1dc00-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1dc00-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1dc00-114">Not supported.</span></span>|
|<span data-ttu-id="1dc00-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1dc00-115">Application</span></span>|<span data-ttu-id="1dc00-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1dc00-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1dc00-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1dc00-117">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="1dc00-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1dc00-118">Request headers</span></span>
|<span data-ttu-id="1dc00-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1dc00-119">Header</span></span>|<span data-ttu-id="1dc00-120">値</span><span class="sxs-lookup"><span data-stu-id="1dc00-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1dc00-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1dc00-121">Authorization</span></span>|<span data-ttu-id="1dc00-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="1dc00-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1dc00-123">承諾</span><span class="sxs-lookup"><span data-stu-id="1dc00-123">Accept</span></span>|<span data-ttu-id="1dc00-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1dc00-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1dc00-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="1dc00-125">Request body</span></span>
<span data-ttu-id="1dc00-126">要求本文で、windowsInformationProtectionAppLockerFile オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="1dc00-126">In the request body, supply a JSON representation for the windowsInformationProtectionAppLockerFile object.</span></span>

<span data-ttu-id="1dc00-127">次の表に、windowsInformationProtectionAppLockerFile の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="1dc00-127">The following table shows the properties that are required when you create the windowsInformationProtectionAppLockerFile.</span></span>

|<span data-ttu-id="1dc00-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1dc00-128">Property</span></span>|<span data-ttu-id="1dc00-129">型</span><span class="sxs-lookup"><span data-stu-id="1dc00-129">Type</span></span>|<span data-ttu-id="1dc00-130">説明</span><span class="sxs-lookup"><span data-stu-id="1dc00-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1dc00-131">displayName</span><span class="sxs-lookup"><span data-stu-id="1dc00-131">displayName</span></span>|<span data-ttu-id="1dc00-132">String</span><span class="sxs-lookup"><span data-stu-id="1dc00-132">String</span></span>|<span data-ttu-id="1dc00-133">フレンドリ名</span><span class="sxs-lookup"><span data-stu-id="1dc00-133">The friendly name</span></span>|
|<span data-ttu-id="1dc00-134">fileHash</span><span class="sxs-lookup"><span data-stu-id="1dc00-134">fileHash</span></span>|<span data-ttu-id="1dc00-135">String</span><span class="sxs-lookup"><span data-stu-id="1dc00-135">String</span></span>|<span data-ttu-id="1dc00-136">ファイルの SHA256 ハッシュ</span><span class="sxs-lookup"><span data-stu-id="1dc00-136">SHA256 hash of the file</span></span>|
|<span data-ttu-id="1dc00-137">file</span><span class="sxs-lookup"><span data-stu-id="1dc00-137">file</span></span>|<span data-ttu-id="1dc00-138">Binary</span><span class="sxs-lookup"><span data-stu-id="1dc00-138">Binary</span></span>|<span data-ttu-id="1dc00-139">バイト配列のファイル</span><span class="sxs-lookup"><span data-stu-id="1dc00-139">File as a byte array</span></span>|
|<span data-ttu-id="1dc00-140">id</span><span class="sxs-lookup"><span data-stu-id="1dc00-140">id</span></span>|<span data-ttu-id="1dc00-141">文字列</span><span class="sxs-lookup"><span data-stu-id="1dc00-141">String</span></span>|<span data-ttu-id="1dc00-142">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="1dc00-142">Key of the entity.</span></span>|
|<span data-ttu-id="1dc00-143">version</span><span class="sxs-lookup"><span data-stu-id="1dc00-143">version</span></span>|<span data-ttu-id="1dc00-144">String</span><span class="sxs-lookup"><span data-stu-id="1dc00-144">String</span></span>|<span data-ttu-id="1dc00-145">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="1dc00-145">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="1dc00-146">応答</span><span class="sxs-lookup"><span data-stu-id="1dc00-146">Response</span></span>
<span data-ttu-id="1dc00-147">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1dc00-147">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1dc00-148">例</span><span class="sxs-lookup"><span data-stu-id="1dc00-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="1dc00-149">要求</span><span class="sxs-lookup"><span data-stu-id="1dc00-149">Request</span></span>
<span data-ttu-id="1dc00-150">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1dc00-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1dc00-151">応答</span><span class="sxs-lookup"><span data-stu-id="1dc00-151">Response</span></span>
<span data-ttu-id="1dc00-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1dc00-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



