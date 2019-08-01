---
title: windowsInformationProtectionAppLearningSummary の更新
description: windowsInformationProtectionAppLearningSummary オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 88d3c49f25c511325b2a598db850b532fc982921
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36023210"
---
# <a name="update-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="12c29-103">windowsInformationProtectionAppLearningSummary の更新</span><span class="sxs-lookup"><span data-stu-id="12c29-103">Update windowsInformationProtectionAppLearningSummary</span></span>

> <span data-ttu-id="12c29-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="12c29-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12c29-105">[windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="12c29-105">Update the properties of a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="12c29-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="12c29-106">Prerequisites</span></span>
<span data-ttu-id="12c29-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="12c29-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12c29-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="12c29-109">Permission type</span></span>|<span data-ttu-id="12c29-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="12c29-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12c29-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="12c29-111">Delegated (work or school account)</span></span>|<span data-ttu-id="12c29-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12c29-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="12c29-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="12c29-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12c29-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="12c29-114">Not supported.</span></span>|
|<span data-ttu-id="12c29-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="12c29-115">Application</span></span>|<span data-ttu-id="12c29-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="12c29-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="12c29-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="12c29-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="12c29-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="12c29-118">Request headers</span></span>
|<span data-ttu-id="12c29-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="12c29-119">Header</span></span>|<span data-ttu-id="12c29-120">値</span><span class="sxs-lookup"><span data-stu-id="12c29-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12c29-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="12c29-121">Authorization</span></span>|<span data-ttu-id="12c29-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="12c29-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12c29-123">承諾</span><span class="sxs-lookup"><span data-stu-id="12c29-123">Accept</span></span>|<span data-ttu-id="12c29-124">application/json</span><span class="sxs-lookup"><span data-stu-id="12c29-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12c29-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="12c29-125">Request body</span></span>
<span data-ttu-id="12c29-126">要求本文で、[windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="12c29-126">In the request body, supply a JSON representation for the [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

<span data-ttu-id="12c29-127">次の表に、[windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="12c29-127">The following table shows the properties that are required when you create the [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span></span>

|<span data-ttu-id="12c29-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="12c29-128">Property</span></span>|<span data-ttu-id="12c29-129">型</span><span class="sxs-lookup"><span data-stu-id="12c29-129">Type</span></span>|<span data-ttu-id="12c29-130">説明</span><span class="sxs-lookup"><span data-stu-id="12c29-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12c29-131">id</span><span class="sxs-lookup"><span data-stu-id="12c29-131">id</span></span>|<span data-ttu-id="12c29-132">String</span><span class="sxs-lookup"><span data-stu-id="12c29-132">String</span></span>|<span data-ttu-id="12c29-133">WindowsInformationProtectionAppLearningSummary の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="12c29-133">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="12c29-134">applicationName</span><span class="sxs-lookup"><span data-stu-id="12c29-134">applicationName</span></span>|<span data-ttu-id="12c29-135">String</span><span class="sxs-lookup"><span data-stu-id="12c29-135">String</span></span>|<span data-ttu-id="12c29-136">アプリケーション名</span><span class="sxs-lookup"><span data-stu-id="12c29-136">Application Name</span></span>|
|<span data-ttu-id="12c29-137">applicationType</span><span class="sxs-lookup"><span data-stu-id="12c29-137">applicationType</span></span>|[<span data-ttu-id="12c29-138">applicationType</span><span class="sxs-lookup"><span data-stu-id="12c29-138">applicationType</span></span>](../resources/intune-wip-applicationtype.md)|<span data-ttu-id="12c29-139">アプリケーションの種類。</span><span class="sxs-lookup"><span data-stu-id="12c29-139">Application Type.</span></span> <span data-ttu-id="12c29-140">可能な値は、`universal`、`desktop` です。</span><span class="sxs-lookup"><span data-stu-id="12c29-140">Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="12c29-141">deviceCount</span><span class="sxs-lookup"><span data-stu-id="12c29-141">deviceCount</span></span>|<span data-ttu-id="12c29-142">Int32</span><span class="sxs-lookup"><span data-stu-id="12c29-142">Int32</span></span>|<span data-ttu-id="12c29-143">デバイス数</span><span class="sxs-lookup"><span data-stu-id="12c29-143">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="12c29-144">応答</span><span class="sxs-lookup"><span data-stu-id="12c29-144">Response</span></span>
<span data-ttu-id="12c29-145">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="12c29-145">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12c29-146">例</span><span class="sxs-lookup"><span data-stu-id="12c29-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="12c29-147">要求</span><span class="sxs-lookup"><span data-stu-id="12c29-147">Request</span></span>
<span data-ttu-id="12c29-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="12c29-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
Content-type: application/json
Content-length: 191

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "applicationName": "Application Name value",
  "applicationType": "desktop",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="12c29-149">応答</span><span class="sxs-lookup"><span data-stu-id="12c29-149">Response</span></span>
<span data-ttu-id="12c29-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="12c29-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



