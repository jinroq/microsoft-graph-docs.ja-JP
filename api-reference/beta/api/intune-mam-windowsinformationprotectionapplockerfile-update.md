---
title: windowsInformationProtectionAppLockerFile の更新
description: windowsInformationProtectionAppLockerFile オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: eee21cf2a7f2ece277ab3435b566d486120a8fc1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399830"
---
# <a name="update-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="88124-103">windowsInformationProtectionAppLockerFile の更新</span><span class="sxs-lookup"><span data-stu-id="88124-103">Update windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="88124-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="88124-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="88124-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="88124-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="88124-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="88124-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88124-107">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="88124-107">Update the properties of a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="88124-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="88124-108">Prerequisites</span></span>
<span data-ttu-id="88124-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="88124-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="88124-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="88124-111">Permission type</span></span>|<span data-ttu-id="88124-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="88124-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88124-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="88124-113">Delegated (work or school account)</span></span>|<span data-ttu-id="88124-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88124-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="88124-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="88124-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88124-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="88124-116">Not supported.</span></span>|
|<span data-ttu-id="88124-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="88124-117">Application</span></span>|<span data-ttu-id="88124-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="88124-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="88124-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="88124-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="88124-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="88124-120">Request headers</span></span>
|<span data-ttu-id="88124-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="88124-121">Header</span></span>|<span data-ttu-id="88124-122">値</span><span class="sxs-lookup"><span data-stu-id="88124-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="88124-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="88124-123">Authorization</span></span>|<span data-ttu-id="88124-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="88124-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="88124-125">Accept</span><span class="sxs-lookup"><span data-stu-id="88124-125">Accept</span></span>|<span data-ttu-id="88124-126">application/json</span><span class="sxs-lookup"><span data-stu-id="88124-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="88124-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="88124-127">Request body</span></span>
<span data-ttu-id="88124-128">要求本文で、[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="88124-128">In the request body, supply a JSON representation for the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

<span data-ttu-id="88124-129">次の表に、[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="88124-129">The following table shows the properties that are required when you create the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span></span>

|<span data-ttu-id="88124-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="88124-130">Property</span></span>|<span data-ttu-id="88124-131">型</span><span class="sxs-lookup"><span data-stu-id="88124-131">Type</span></span>|<span data-ttu-id="88124-132">説明</span><span class="sxs-lookup"><span data-stu-id="88124-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88124-133">displayName</span><span class="sxs-lookup"><span data-stu-id="88124-133">displayName</span></span>|<span data-ttu-id="88124-134">String</span><span class="sxs-lookup"><span data-stu-id="88124-134">String</span></span>|<span data-ttu-id="88124-135">フレンドリ名</span><span class="sxs-lookup"><span data-stu-id="88124-135">The friendly name</span></span>|
|<span data-ttu-id="88124-136">fileHash</span><span class="sxs-lookup"><span data-stu-id="88124-136">fileHash</span></span>|<span data-ttu-id="88124-137">String</span><span class="sxs-lookup"><span data-stu-id="88124-137">String</span></span>|<span data-ttu-id="88124-138">ファイルの SHA256 ハッシュ</span><span class="sxs-lookup"><span data-stu-id="88124-138">SHA256 hash of the file</span></span>|
|<span data-ttu-id="88124-139">file</span><span class="sxs-lookup"><span data-stu-id="88124-139">file</span></span>|<span data-ttu-id="88124-140">Binary</span><span class="sxs-lookup"><span data-stu-id="88124-140">Binary</span></span>|<span data-ttu-id="88124-141">バイト配列のファイル</span><span class="sxs-lookup"><span data-stu-id="88124-141">File as a byte array</span></span>|
|<span data-ttu-id="88124-142">id</span><span class="sxs-lookup"><span data-stu-id="88124-142">id</span></span>|<span data-ttu-id="88124-143">String</span><span class="sxs-lookup"><span data-stu-id="88124-143">String</span></span>|<span data-ttu-id="88124-144">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="88124-144">Key of the entity.</span></span>|
|<span data-ttu-id="88124-145">version</span><span class="sxs-lookup"><span data-stu-id="88124-145">version</span></span>|<span data-ttu-id="88124-146">String</span><span class="sxs-lookup"><span data-stu-id="88124-146">String</span></span>|<span data-ttu-id="88124-147">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="88124-147">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="88124-148">応答</span><span class="sxs-lookup"><span data-stu-id="88124-148">Response</span></span>
<span data-ttu-id="88124-149">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="88124-149">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88124-150">例</span><span class="sxs-lookup"><span data-stu-id="88124-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="88124-151">要求</span><span class="sxs-lookup"><span data-stu-id="88124-151">Request</span></span>
<span data-ttu-id="88124-152">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="88124-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="88124-153">応答</span><span class="sxs-lookup"><span data-stu-id="88124-153">Response</span></span>
<span data-ttu-id="88124-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="88124-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




