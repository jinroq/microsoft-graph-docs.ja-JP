---
title: windowsInformationProtectionAppLockerFile の作成
description: 新しい windowsInformationProtectionAppLockerFile オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9399f23590bee975506a2972f6ba3bc0fa8c3c07
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30975785"
---
# <a name="create-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="66e0c-103">windowsInformationProtectionAppLockerFile の作成</span><span class="sxs-lookup"><span data-stu-id="66e0c-103">Create windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="66e0c-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="66e0c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="66e0c-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="66e0c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66e0c-106">新しい [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="66e0c-106">Create a new [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="66e0c-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="66e0c-107">Prerequisites</span></span>
<span data-ttu-id="66e0c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="66e0c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66e0c-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="66e0c-110">Permission type</span></span>|<span data-ttu-id="66e0c-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="66e0c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="66e0c-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="66e0c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="66e0c-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66e0c-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="66e0c-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="66e0c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="66e0c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="66e0c-115">Not supported.</span></span>|
|<span data-ttu-id="66e0c-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="66e0c-116">Application</span></span>|<span data-ttu-id="66e0c-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="66e0c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="66e0c-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="66e0c-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="66e0c-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="66e0c-119">Request headers</span></span>
|<span data-ttu-id="66e0c-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="66e0c-120">Header</span></span>|<span data-ttu-id="66e0c-121">値</span><span class="sxs-lookup"><span data-stu-id="66e0c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="66e0c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="66e0c-122">Authorization</span></span>|<span data-ttu-id="66e0c-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="66e0c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="66e0c-124">承諾</span><span class="sxs-lookup"><span data-stu-id="66e0c-124">Accept</span></span>|<span data-ttu-id="66e0c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="66e0c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="66e0c-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="66e0c-126">Request body</span></span>
<span data-ttu-id="66e0c-127">要求本文で、windowsInformationProtectionAppLockerFile オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="66e0c-127">In the request body, supply a JSON representation for the windowsInformationProtectionAppLockerFile object.</span></span>

<span data-ttu-id="66e0c-128">次の表に、windowsInformationProtectionAppLockerFile の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="66e0c-128">The following table shows the properties that are required when you create the windowsInformationProtectionAppLockerFile.</span></span>

|<span data-ttu-id="66e0c-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="66e0c-129">Property</span></span>|<span data-ttu-id="66e0c-130">型</span><span class="sxs-lookup"><span data-stu-id="66e0c-130">Type</span></span>|<span data-ttu-id="66e0c-131">説明</span><span class="sxs-lookup"><span data-stu-id="66e0c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66e0c-132">displayName</span><span class="sxs-lookup"><span data-stu-id="66e0c-132">displayName</span></span>|<span data-ttu-id="66e0c-133">String</span><span class="sxs-lookup"><span data-stu-id="66e0c-133">String</span></span>|<span data-ttu-id="66e0c-134">フレンドリ名</span><span class="sxs-lookup"><span data-stu-id="66e0c-134">The friendly name</span></span>|
|<span data-ttu-id="66e0c-135">fileHash</span><span class="sxs-lookup"><span data-stu-id="66e0c-135">fileHash</span></span>|<span data-ttu-id="66e0c-136">String</span><span class="sxs-lookup"><span data-stu-id="66e0c-136">String</span></span>|<span data-ttu-id="66e0c-137">ファイルの SHA256 ハッシュ</span><span class="sxs-lookup"><span data-stu-id="66e0c-137">SHA256 hash of the file</span></span>|
|<span data-ttu-id="66e0c-138">file</span><span class="sxs-lookup"><span data-stu-id="66e0c-138">file</span></span>|<span data-ttu-id="66e0c-139">Binary</span><span class="sxs-lookup"><span data-stu-id="66e0c-139">Binary</span></span>|<span data-ttu-id="66e0c-140">バイト配列のファイル</span><span class="sxs-lookup"><span data-stu-id="66e0c-140">File as a byte array</span></span>|
|<span data-ttu-id="66e0c-141">id</span><span class="sxs-lookup"><span data-stu-id="66e0c-141">id</span></span>|<span data-ttu-id="66e0c-142">String</span><span class="sxs-lookup"><span data-stu-id="66e0c-142">String</span></span>|<span data-ttu-id="66e0c-143">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="66e0c-143">Key of the entity.</span></span>|
|<span data-ttu-id="66e0c-144">version</span><span class="sxs-lookup"><span data-stu-id="66e0c-144">version</span></span>|<span data-ttu-id="66e0c-145">String</span><span class="sxs-lookup"><span data-stu-id="66e0c-145">String</span></span>|<span data-ttu-id="66e0c-146">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="66e0c-146">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="66e0c-147">応答</span><span class="sxs-lookup"><span data-stu-id="66e0c-147">Response</span></span>
<span data-ttu-id="66e0c-148">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="66e0c-148">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66e0c-149">例</span><span class="sxs-lookup"><span data-stu-id="66e0c-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="66e0c-150">要求</span><span class="sxs-lookup"><span data-stu-id="66e0c-150">Request</span></span>
<span data-ttu-id="66e0c-151">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="66e0c-151">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles
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

### <a name="response"></a><span data-ttu-id="66e0c-152">応答</span><span class="sxs-lookup"><span data-stu-id="66e0c-152">Response</span></span>
<span data-ttu-id="66e0c-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="66e0c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




