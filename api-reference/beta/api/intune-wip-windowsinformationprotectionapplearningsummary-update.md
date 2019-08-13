---
title: windowsInformationProtectionAppLearningSummary の更新
description: windowsInformationProtectionAppLearningSummary オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 372e99c3557022c4e1856c496fc6068e59ba8169
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36343028"
---
# <a name="update-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="09a3d-103">windowsInformationProtectionAppLearningSummary の更新</span><span class="sxs-lookup"><span data-stu-id="09a3d-103">Update windowsInformationProtectionAppLearningSummary</span></span>

> <span data-ttu-id="09a3d-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="09a3d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="09a3d-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="09a3d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09a3d-106">[windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="09a3d-106">Update the properties of a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="09a3d-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="09a3d-107">Prerequisites</span></span>
<span data-ttu-id="09a3d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="09a3d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09a3d-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="09a3d-110">Permission type</span></span>|<span data-ttu-id="09a3d-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="09a3d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="09a3d-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="09a3d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="09a3d-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09a3d-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="09a3d-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="09a3d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="09a3d-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="09a3d-115">Not supported.</span></span>|
|<span data-ttu-id="09a3d-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="09a3d-116">Application</span></span>|<span data-ttu-id="09a3d-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09a3d-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="09a3d-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="09a3d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="09a3d-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="09a3d-119">Request headers</span></span>
|<span data-ttu-id="09a3d-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="09a3d-120">Header</span></span>|<span data-ttu-id="09a3d-121">値</span><span class="sxs-lookup"><span data-stu-id="09a3d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="09a3d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="09a3d-122">Authorization</span></span>|<span data-ttu-id="09a3d-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="09a3d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="09a3d-124">承諾</span><span class="sxs-lookup"><span data-stu-id="09a3d-124">Accept</span></span>|<span data-ttu-id="09a3d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="09a3d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="09a3d-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="09a3d-126">Request body</span></span>
<span data-ttu-id="09a3d-127">要求本文で、[windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="09a3d-127">In the request body, supply a JSON representation for the [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

<span data-ttu-id="09a3d-128">次の表に、[windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="09a3d-128">The following table shows the properties that are required when you create the [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span></span>

|<span data-ttu-id="09a3d-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="09a3d-129">Property</span></span>|<span data-ttu-id="09a3d-130">型</span><span class="sxs-lookup"><span data-stu-id="09a3d-130">Type</span></span>|<span data-ttu-id="09a3d-131">説明</span><span class="sxs-lookup"><span data-stu-id="09a3d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09a3d-132">id</span><span class="sxs-lookup"><span data-stu-id="09a3d-132">id</span></span>|<span data-ttu-id="09a3d-133">String</span><span class="sxs-lookup"><span data-stu-id="09a3d-133">String</span></span>|<span data-ttu-id="09a3d-134">WindowsInformationProtectionAppLearningSummary の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="09a3d-134">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="09a3d-135">applicationName</span><span class="sxs-lookup"><span data-stu-id="09a3d-135">applicationName</span></span>|<span data-ttu-id="09a3d-136">String</span><span class="sxs-lookup"><span data-stu-id="09a3d-136">String</span></span>|<span data-ttu-id="09a3d-137">アプリケーション名</span><span class="sxs-lookup"><span data-stu-id="09a3d-137">Application Name</span></span>|
|<span data-ttu-id="09a3d-138">applicationType</span><span class="sxs-lookup"><span data-stu-id="09a3d-138">applicationType</span></span>|[<span data-ttu-id="09a3d-139">applicationType</span><span class="sxs-lookup"><span data-stu-id="09a3d-139">applicationType</span></span>](../resources/intune-wip-applicationtype.md)|<span data-ttu-id="09a3d-140">アプリケーションの種類。</span><span class="sxs-lookup"><span data-stu-id="09a3d-140">Application Type.</span></span> <span data-ttu-id="09a3d-141">可能な値は、`universal`、`desktop` です。</span><span class="sxs-lookup"><span data-stu-id="09a3d-141">Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="09a3d-142">deviceCount</span><span class="sxs-lookup"><span data-stu-id="09a3d-142">deviceCount</span></span>|<span data-ttu-id="09a3d-143">Int32</span><span class="sxs-lookup"><span data-stu-id="09a3d-143">Int32</span></span>|<span data-ttu-id="09a3d-144">デバイス数</span><span class="sxs-lookup"><span data-stu-id="09a3d-144">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="09a3d-145">応答</span><span class="sxs-lookup"><span data-stu-id="09a3d-145">Response</span></span>
<span data-ttu-id="09a3d-146">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="09a3d-146">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09a3d-147">例</span><span class="sxs-lookup"><span data-stu-id="09a3d-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="09a3d-148">要求</span><span class="sxs-lookup"><span data-stu-id="09a3d-148">Request</span></span>
<span data-ttu-id="09a3d-149">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="09a3d-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
Content-type: application/json
Content-length: 191

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "applicationName": "Application Name value",
  "applicationType": "desktop",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="09a3d-150">応答</span><span class="sxs-lookup"><span data-stu-id="09a3d-150">Response</span></span>
<span data-ttu-id="09a3d-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="09a3d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






