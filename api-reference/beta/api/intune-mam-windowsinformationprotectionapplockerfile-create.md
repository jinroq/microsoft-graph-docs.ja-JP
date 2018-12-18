---
title: windowsInformationProtectionAppLockerFile の作成
description: 新しい windowsInformationProtectionAppLockerFile オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: f2cbed922d6f2ac130169e5d9c85e3a5231184a5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27317123"
---
# <a name="create-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="2851c-103">windowsInformationProtectionAppLockerFile の作成</span><span class="sxs-lookup"><span data-stu-id="2851c-103">Create windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="2851c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2851c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2851c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2851c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2851c-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2851c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2851c-107">新しい [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="2851c-107">Create a new [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2851c-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="2851c-108">Prerequisites</span></span>
<span data-ttu-id="2851c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2851c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2851c-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2851c-111">Permission type</span></span>|<span data-ttu-id="2851c-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2851c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2851c-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2851c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2851c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2851c-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2851c-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2851c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2851c-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2851c-116">Not supported.</span></span>|
|<span data-ttu-id="2851c-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2851c-117">Application</span></span>|<span data-ttu-id="2851c-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2851c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2851c-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2851c-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="2851c-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2851c-120">Request headers</span></span>
|<span data-ttu-id="2851c-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2851c-121">Header</span></span>|<span data-ttu-id="2851c-122">値</span><span class="sxs-lookup"><span data-stu-id="2851c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2851c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2851c-123">Authorization</span></span>|<span data-ttu-id="2851c-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="2851c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2851c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2851c-125">Accept</span></span>|<span data-ttu-id="2851c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2851c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2851c-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="2851c-127">Request body</span></span>
<span data-ttu-id="2851c-128">要求本文で、windowsInformationProtectionAppLockerFile オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="2851c-128">In the request body, supply a JSON representation for the windowsInformationProtectionAppLockerFile object.</span></span>

<span data-ttu-id="2851c-129">次の表に、windowsInformationProtectionAppLockerFile の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="2851c-129">The following table shows the properties that are required when you create the windowsInformationProtectionAppLockerFile.</span></span>

|<span data-ttu-id="2851c-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2851c-130">Property</span></span>|<span data-ttu-id="2851c-131">種類</span><span class="sxs-lookup"><span data-stu-id="2851c-131">Type</span></span>|<span data-ttu-id="2851c-132">説明</span><span class="sxs-lookup"><span data-stu-id="2851c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2851c-133">displayName</span><span class="sxs-lookup"><span data-stu-id="2851c-133">displayName</span></span>|<span data-ttu-id="2851c-134">String</span><span class="sxs-lookup"><span data-stu-id="2851c-134">String</span></span>|<span data-ttu-id="2851c-135">フレンドリ名</span><span class="sxs-lookup"><span data-stu-id="2851c-135">The friendly name</span></span>|
|<span data-ttu-id="2851c-136">fileHash</span><span class="sxs-lookup"><span data-stu-id="2851c-136">fileHash</span></span>|<span data-ttu-id="2851c-137">String</span><span class="sxs-lookup"><span data-stu-id="2851c-137">String</span></span>|<span data-ttu-id="2851c-138">ファイルの SHA256 ハッシュ</span><span class="sxs-lookup"><span data-stu-id="2851c-138">SHA256 hash of the file</span></span>|
|<span data-ttu-id="2851c-139">file</span><span class="sxs-lookup"><span data-stu-id="2851c-139">file</span></span>|<span data-ttu-id="2851c-140">Binary</span><span class="sxs-lookup"><span data-stu-id="2851c-140">Binary</span></span>|<span data-ttu-id="2851c-141">バイト配列のファイル</span><span class="sxs-lookup"><span data-stu-id="2851c-141">File as a byte array</span></span>|
|<span data-ttu-id="2851c-142">id</span><span class="sxs-lookup"><span data-stu-id="2851c-142">id</span></span>|<span data-ttu-id="2851c-143">String</span><span class="sxs-lookup"><span data-stu-id="2851c-143">String</span></span>|<span data-ttu-id="2851c-144">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="2851c-144">Key of the entity.</span></span>|
|<span data-ttu-id="2851c-145">version</span><span class="sxs-lookup"><span data-stu-id="2851c-145">version</span></span>|<span data-ttu-id="2851c-146">String</span><span class="sxs-lookup"><span data-stu-id="2851c-146">String</span></span>|<span data-ttu-id="2851c-147">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="2851c-147">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="2851c-148">応答</span><span class="sxs-lookup"><span data-stu-id="2851c-148">Response</span></span>
<span data-ttu-id="2851c-149">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2851c-149">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2851c-150">例</span><span class="sxs-lookup"><span data-stu-id="2851c-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="2851c-151">要求</span><span class="sxs-lookup"><span data-stu-id="2851c-151">Request</span></span>
<span data-ttu-id="2851c-152">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2851c-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2851c-153">応答</span><span class="sxs-lookup"><span data-stu-id="2851c-153">Response</span></span>
<span data-ttu-id="2851c-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2851c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





