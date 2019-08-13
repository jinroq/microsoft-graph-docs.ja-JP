---
title: windowsInformationProtectionAppLockerFile の更新
description: windowsInformationProtectionAppLockerFile オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 761b4638e261319c99be7e3135f04100de2516f6
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36353548"
---
# <a name="update-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="601fb-103">windowsInformationProtectionAppLockerFile の更新</span><span class="sxs-lookup"><span data-stu-id="601fb-103">Update windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="601fb-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="601fb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="601fb-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="601fb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="601fb-106">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="601fb-106">Update the properties of a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="601fb-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="601fb-107">Prerequisites</span></span>
<span data-ttu-id="601fb-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="601fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="601fb-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="601fb-110">Permission type</span></span>|<span data-ttu-id="601fb-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="601fb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="601fb-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="601fb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="601fb-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="601fb-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="601fb-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="601fb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="601fb-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="601fb-115">Not supported.</span></span>|
|<span data-ttu-id="601fb-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="601fb-116">Application</span></span>|<span data-ttu-id="601fb-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="601fb-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="601fb-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="601fb-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="601fb-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="601fb-119">Request headers</span></span>
|<span data-ttu-id="601fb-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="601fb-120">Header</span></span>|<span data-ttu-id="601fb-121">値</span><span class="sxs-lookup"><span data-stu-id="601fb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="601fb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="601fb-122">Authorization</span></span>|<span data-ttu-id="601fb-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="601fb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="601fb-124">承諾</span><span class="sxs-lookup"><span data-stu-id="601fb-124">Accept</span></span>|<span data-ttu-id="601fb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="601fb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="601fb-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="601fb-126">Request body</span></span>
<span data-ttu-id="601fb-127">要求本文で、[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="601fb-127">In the request body, supply a JSON representation for the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

<span data-ttu-id="601fb-128">次の表に、[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="601fb-128">The following table shows the properties that are required when you create the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span></span>

|<span data-ttu-id="601fb-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="601fb-129">Property</span></span>|<span data-ttu-id="601fb-130">型</span><span class="sxs-lookup"><span data-stu-id="601fb-130">Type</span></span>|<span data-ttu-id="601fb-131">説明</span><span class="sxs-lookup"><span data-stu-id="601fb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="601fb-132">displayName</span><span class="sxs-lookup"><span data-stu-id="601fb-132">displayName</span></span>|<span data-ttu-id="601fb-133">String</span><span class="sxs-lookup"><span data-stu-id="601fb-133">String</span></span>|<span data-ttu-id="601fb-134">フレンドリ名</span><span class="sxs-lookup"><span data-stu-id="601fb-134">The friendly name</span></span>|
|<span data-ttu-id="601fb-135">fileHash</span><span class="sxs-lookup"><span data-stu-id="601fb-135">fileHash</span></span>|<span data-ttu-id="601fb-136">String</span><span class="sxs-lookup"><span data-stu-id="601fb-136">String</span></span>|<span data-ttu-id="601fb-137">ファイルの SHA256 ハッシュ</span><span class="sxs-lookup"><span data-stu-id="601fb-137">SHA256 hash of the file</span></span>|
|<span data-ttu-id="601fb-138">file</span><span class="sxs-lookup"><span data-stu-id="601fb-138">file</span></span>|<span data-ttu-id="601fb-139">Binary</span><span class="sxs-lookup"><span data-stu-id="601fb-139">Binary</span></span>|<span data-ttu-id="601fb-140">バイト配列のファイル</span><span class="sxs-lookup"><span data-stu-id="601fb-140">File as a byte array</span></span>|
|<span data-ttu-id="601fb-141">id</span><span class="sxs-lookup"><span data-stu-id="601fb-141">id</span></span>|<span data-ttu-id="601fb-142">文字列</span><span class="sxs-lookup"><span data-stu-id="601fb-142">String</span></span>|<span data-ttu-id="601fb-143">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="601fb-143">Key of the entity.</span></span>|
|<span data-ttu-id="601fb-144">version</span><span class="sxs-lookup"><span data-stu-id="601fb-144">version</span></span>|<span data-ttu-id="601fb-145">String</span><span class="sxs-lookup"><span data-stu-id="601fb-145">String</span></span>|<span data-ttu-id="601fb-146">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="601fb-146">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="601fb-147">応答</span><span class="sxs-lookup"><span data-stu-id="601fb-147">Response</span></span>
<span data-ttu-id="601fb-148">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="601fb-148">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="601fb-149">例</span><span class="sxs-lookup"><span data-stu-id="601fb-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="601fb-150">要求</span><span class="sxs-lookup"><span data-stu-id="601fb-150">Request</span></span>
<span data-ttu-id="601fb-151">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="601fb-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
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

### <a name="response"></a><span data-ttu-id="601fb-152">応答</span><span class="sxs-lookup"><span data-stu-id="601fb-152">Response</span></span>
<span data-ttu-id="601fb-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="601fb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






