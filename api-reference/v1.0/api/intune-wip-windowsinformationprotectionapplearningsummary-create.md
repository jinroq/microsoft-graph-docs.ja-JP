---
title: windowsInformationProtectionAppLearningSummary の作成
description: 新しい windowsInformationProtectionAppLearningSummary オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 43f36e67ea0d1ec46708bcac1e5ecdf528f35c5b
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30959475"
---
# <a name="create-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="51484-103">windowsInformationProtectionAppLearningSummary の作成</span><span class="sxs-lookup"><span data-stu-id="51484-103">Create windowsInformationProtectionAppLearningSummary</span></span>

> <span data-ttu-id="51484-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="51484-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51484-105">新しい [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="51484-105">Create a new [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="51484-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="51484-106">Prerequisites</span></span>
<span data-ttu-id="51484-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="51484-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51484-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="51484-109">Permission type</span></span>|<span data-ttu-id="51484-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="51484-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51484-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="51484-111">Delegated (work or school account)</span></span>|<span data-ttu-id="51484-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51484-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="51484-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="51484-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51484-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="51484-114">Not supported.</span></span>|
|<span data-ttu-id="51484-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="51484-115">Application</span></span>|<span data-ttu-id="51484-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="51484-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="51484-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="51484-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionAppLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="51484-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="51484-118">Request headers</span></span>
|<span data-ttu-id="51484-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="51484-119">Header</span></span>|<span data-ttu-id="51484-120">値</span><span class="sxs-lookup"><span data-stu-id="51484-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51484-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="51484-121">Authorization</span></span>|<span data-ttu-id="51484-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="51484-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51484-123">承諾</span><span class="sxs-lookup"><span data-stu-id="51484-123">Accept</span></span>|<span data-ttu-id="51484-124">application/json</span><span class="sxs-lookup"><span data-stu-id="51484-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51484-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="51484-125">Request body</span></span>
<span data-ttu-id="51484-126">要求本文で、windowsInformationProtectionAppLearningSummary オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="51484-126">In the request body, supply a JSON representation for the windowsInformationProtectionAppLearningSummary object.</span></span>

<span data-ttu-id="51484-127">次の表に、windowsInformationProtectionAppLearningSummary の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="51484-127">The following table shows the properties that are required when you create the windowsInformationProtectionAppLearningSummary.</span></span>

|<span data-ttu-id="51484-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="51484-128">Property</span></span>|<span data-ttu-id="51484-129">型</span><span class="sxs-lookup"><span data-stu-id="51484-129">Type</span></span>|<span data-ttu-id="51484-130">説明</span><span class="sxs-lookup"><span data-stu-id="51484-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51484-131">id</span><span class="sxs-lookup"><span data-stu-id="51484-131">id</span></span>|<span data-ttu-id="51484-132">String</span><span class="sxs-lookup"><span data-stu-id="51484-132">String</span></span>|<span data-ttu-id="51484-133">WindowsInformationProtectionAppLearningSummary の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="51484-133">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="51484-134">applicationName</span><span class="sxs-lookup"><span data-stu-id="51484-134">applicationName</span></span>|<span data-ttu-id="51484-135">String</span><span class="sxs-lookup"><span data-stu-id="51484-135">String</span></span>|<span data-ttu-id="51484-136">アプリケーション名</span><span class="sxs-lookup"><span data-stu-id="51484-136">Application Name</span></span>|
|<span data-ttu-id="51484-137">applicationType</span><span class="sxs-lookup"><span data-stu-id="51484-137">applicationType</span></span>|[<span data-ttu-id="51484-138">applicationType</span><span class="sxs-lookup"><span data-stu-id="51484-138">applicationType</span></span>](../resources/intune-wip-applicationtype.md)|<span data-ttu-id="51484-139">アプリケーションの種類。</span><span class="sxs-lookup"><span data-stu-id="51484-139">Application Type.</span></span> <span data-ttu-id="51484-140">可能な値は、`universal`、`desktop` です。</span><span class="sxs-lookup"><span data-stu-id="51484-140">Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="51484-141">deviceCount</span><span class="sxs-lookup"><span data-stu-id="51484-141">deviceCount</span></span>|<span data-ttu-id="51484-142">Int32</span><span class="sxs-lookup"><span data-stu-id="51484-142">Int32</span></span>|<span data-ttu-id="51484-143">デバイス数</span><span class="sxs-lookup"><span data-stu-id="51484-143">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="51484-144">応答</span><span class="sxs-lookup"><span data-stu-id="51484-144">Response</span></span>
<span data-ttu-id="51484-145">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="51484-145">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51484-146">例</span><span class="sxs-lookup"><span data-stu-id="51484-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="51484-147">要求</span><span class="sxs-lookup"><span data-stu-id="51484-147">Request</span></span>
<span data-ttu-id="51484-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="51484-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionAppLearningSummaries
Content-type: application/json
Content-length: 191

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "applicationName": "Application Name value",
  "applicationType": "desktop",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="51484-149">応答</span><span class="sxs-lookup"><span data-stu-id="51484-149">Response</span></span>
<span data-ttu-id="51484-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="51484-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 240

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "id": "063baf50-af50-063b-50af-3b0650af3b06",
  "applicationName": "Application Name value",
  "applicationType": "desktop",
  "deviceCount": 11
}
```



