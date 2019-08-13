---
title: windowsInformationProtectionNetworkLearningSummary の更新
description: windowsInformationProtectionNetworkLearningSummary オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2363383f51da57eec40382d2086a9c82c22f0de0
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36347116"
---
# <a name="update-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="52776-103">windowsInformationProtectionNetworkLearningSummary の更新</span><span class="sxs-lookup"><span data-stu-id="52776-103">Update windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="52776-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="52776-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="52776-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="52776-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52776-106">[windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="52776-106">Update the properties of a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="52776-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="52776-107">Prerequisites</span></span>
<span data-ttu-id="52776-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="52776-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52776-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="52776-110">Permission type</span></span>|<span data-ttu-id="52776-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="52776-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="52776-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="52776-112">Delegated (work or school account)</span></span>|<span data-ttu-id="52776-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52776-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="52776-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="52776-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="52776-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="52776-115">Not supported.</span></span>|
|<span data-ttu-id="52776-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="52776-116">Application</span></span>|<span data-ttu-id="52776-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52776-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="52776-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="52776-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="52776-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="52776-119">Request headers</span></span>
|<span data-ttu-id="52776-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="52776-120">Header</span></span>|<span data-ttu-id="52776-121">値</span><span class="sxs-lookup"><span data-stu-id="52776-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="52776-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="52776-122">Authorization</span></span>|<span data-ttu-id="52776-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="52776-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="52776-124">承諾</span><span class="sxs-lookup"><span data-stu-id="52776-124">Accept</span></span>|<span data-ttu-id="52776-125">application/json</span><span class="sxs-lookup"><span data-stu-id="52776-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="52776-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="52776-126">Request body</span></span>
<span data-ttu-id="52776-127">要求本文で、[windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="52776-127">In the request body, supply a JSON representation for the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

<span data-ttu-id="52776-128">次の表に、[windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="52776-128">The following table shows the properties that are required when you create the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span></span>

|<span data-ttu-id="52776-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="52776-129">Property</span></span>|<span data-ttu-id="52776-130">型</span><span class="sxs-lookup"><span data-stu-id="52776-130">Type</span></span>|<span data-ttu-id="52776-131">説明</span><span class="sxs-lookup"><span data-stu-id="52776-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52776-132">id</span><span class="sxs-lookup"><span data-stu-id="52776-132">id</span></span>|<span data-ttu-id="52776-133">String</span><span class="sxs-lookup"><span data-stu-id="52776-133">String</span></span>|<span data-ttu-id="52776-134">WindowsInformationProtectionNetworkLearningSummary の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="52776-134">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="52776-135">url</span><span class="sxs-lookup"><span data-stu-id="52776-135">url</span></span>|<span data-ttu-id="52776-136">String</span><span class="sxs-lookup"><span data-stu-id="52776-136">String</span></span>|<span data-ttu-id="52776-137">Web サイト URL</span><span class="sxs-lookup"><span data-stu-id="52776-137">Website url</span></span>|
|<span data-ttu-id="52776-138">deviceCount</span><span class="sxs-lookup"><span data-stu-id="52776-138">deviceCount</span></span>|<span data-ttu-id="52776-139">Int32</span><span class="sxs-lookup"><span data-stu-id="52776-139">Int32</span></span>|<span data-ttu-id="52776-140">デバイス数</span><span class="sxs-lookup"><span data-stu-id="52776-140">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="52776-141">応答</span><span class="sxs-lookup"><span data-stu-id="52776-141">Response</span></span>
<span data-ttu-id="52776-142">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="52776-142">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52776-143">例</span><span class="sxs-lookup"><span data-stu-id="52776-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="52776-144">要求</span><span class="sxs-lookup"><span data-stu-id="52776-144">Request</span></span>
<span data-ttu-id="52776-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="52776-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
Content-type: application/json
Content-length: 137

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "url": "Url value",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="52776-146">応答</span><span class="sxs-lookup"><span data-stu-id="52776-146">Response</span></span>
<span data-ttu-id="52776-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="52776-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 186

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "id": "242108f7-08f7-2421-f708-2124f7082124",
  "url": "Url value",
  "deviceCount": 11
}
```






