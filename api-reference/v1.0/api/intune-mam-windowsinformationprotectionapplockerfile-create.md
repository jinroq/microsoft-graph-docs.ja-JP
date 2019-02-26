---
title: windowsInformationProtectionAppLockerFile の作成
description: 新しい windowsInformationProtectionAppLockerFile オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6f3b411e680a3df86b86517f63c8055cec8e4f17
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261839"
---
# <a name="create-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="6696c-103">windowsInformationProtectionAppLockerFile の作成</span><span class="sxs-lookup"><span data-stu-id="6696c-103">Create windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="6696c-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6696c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6696c-105">新しい [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="6696c-105">Create a new [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6696c-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="6696c-106">Prerequisites</span></span>
<span data-ttu-id="6696c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6696c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6696c-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6696c-109">Permission type</span></span>|<span data-ttu-id="6696c-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6696c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6696c-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6696c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6696c-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6696c-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6696c-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6696c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6696c-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6696c-114">Not supported.</span></span>|
|<span data-ttu-id="6696c-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6696c-115">Application</span></span>|<span data-ttu-id="6696c-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6696c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6696c-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6696c-117">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="6696c-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6696c-118">Request headers</span></span>
|<span data-ttu-id="6696c-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6696c-119">Header</span></span>|<span data-ttu-id="6696c-120">値</span><span class="sxs-lookup"><span data-stu-id="6696c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6696c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6696c-121">Authorization</span></span>|<span data-ttu-id="6696c-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="6696c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6696c-123">承諾</span><span class="sxs-lookup"><span data-stu-id="6696c-123">Accept</span></span>|<span data-ttu-id="6696c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6696c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6696c-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="6696c-125">Request body</span></span>
<span data-ttu-id="6696c-126">要求本文で、windowsInformationProtectionAppLockerFile オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="6696c-126">In the request body, supply a JSON representation for the windowsInformationProtectionAppLockerFile object.</span></span>

<span data-ttu-id="6696c-127">次の表に、windowsInformationProtectionAppLockerFile の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="6696c-127">The following table shows the properties that are required when you create the windowsInformationProtectionAppLockerFile.</span></span>

|<span data-ttu-id="6696c-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6696c-128">Property</span></span>|<span data-ttu-id="6696c-129">型</span><span class="sxs-lookup"><span data-stu-id="6696c-129">Type</span></span>|<span data-ttu-id="6696c-130">説明</span><span class="sxs-lookup"><span data-stu-id="6696c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6696c-131">displayName</span><span class="sxs-lookup"><span data-stu-id="6696c-131">displayName</span></span>|<span data-ttu-id="6696c-132">String</span><span class="sxs-lookup"><span data-stu-id="6696c-132">String</span></span>|<span data-ttu-id="6696c-133">フレンドリ名</span><span class="sxs-lookup"><span data-stu-id="6696c-133">The friendly name</span></span>|
|<span data-ttu-id="6696c-134">fileHash</span><span class="sxs-lookup"><span data-stu-id="6696c-134">fileHash</span></span>|<span data-ttu-id="6696c-135">String</span><span class="sxs-lookup"><span data-stu-id="6696c-135">String</span></span>|<span data-ttu-id="6696c-136">ファイルの SHA256 ハッシュ</span><span class="sxs-lookup"><span data-stu-id="6696c-136">SHA256 hash of the file</span></span>|
|<span data-ttu-id="6696c-137">file</span><span class="sxs-lookup"><span data-stu-id="6696c-137">file</span></span>|<span data-ttu-id="6696c-138">Binary</span><span class="sxs-lookup"><span data-stu-id="6696c-138">Binary</span></span>|<span data-ttu-id="6696c-139">バイト配列のファイル</span><span class="sxs-lookup"><span data-stu-id="6696c-139">File as a byte array</span></span>|
|<span data-ttu-id="6696c-140">id</span><span class="sxs-lookup"><span data-stu-id="6696c-140">id</span></span>|<span data-ttu-id="6696c-141">文字列</span><span class="sxs-lookup"><span data-stu-id="6696c-141">String</span></span>|<span data-ttu-id="6696c-142">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="6696c-142">Key of the entity.</span></span>|
|<span data-ttu-id="6696c-143">version</span><span class="sxs-lookup"><span data-stu-id="6696c-143">version</span></span>|<span data-ttu-id="6696c-144">String</span><span class="sxs-lookup"><span data-stu-id="6696c-144">String</span></span>|<span data-ttu-id="6696c-145">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="6696c-145">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="6696c-146">応答</span><span class="sxs-lookup"><span data-stu-id="6696c-146">Response</span></span>
<span data-ttu-id="6696c-147">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6696c-147">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6696c-148">例</span><span class="sxs-lookup"><span data-stu-id="6696c-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="6696c-149">要求</span><span class="sxs-lookup"><span data-stu-id="6696c-149">Request</span></span>
<span data-ttu-id="6696c-150">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6696c-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6696c-151">応答</span><span class="sxs-lookup"><span data-stu-id="6696c-151">Response</span></span>
<span data-ttu-id="6696c-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6696c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



