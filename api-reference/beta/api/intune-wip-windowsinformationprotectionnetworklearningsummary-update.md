---
title: windowsInformationProtectionNetworkLearningSummary の更新
description: windowsInformationProtectionNetworkLearningSummary オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c971045fe876663b19b1a0a09991d37bd7e6e94c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30157443"
---
# <a name="update-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="7ac49-103">windowsInformationProtectionNetworkLearningSummary の更新</span><span class="sxs-lookup"><span data-stu-id="7ac49-103">Update windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="7ac49-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7ac49-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7ac49-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7ac49-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ac49-106">[windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="7ac49-106">Update the properties of a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7ac49-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="7ac49-107">Prerequisites</span></span>
<span data-ttu-id="7ac49-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7ac49-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7ac49-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7ac49-110">Permission type</span></span>|<span data-ttu-id="7ac49-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7ac49-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7ac49-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7ac49-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7ac49-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ac49-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7ac49-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7ac49-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7ac49-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7ac49-115">Not supported.</span></span>|
|<span data-ttu-id="7ac49-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7ac49-116">Application</span></span>|<span data-ttu-id="7ac49-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7ac49-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7ac49-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7ac49-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="7ac49-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7ac49-119">Request headers</span></span>
|<span data-ttu-id="7ac49-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7ac49-120">Header</span></span>|<span data-ttu-id="7ac49-121">値</span><span class="sxs-lookup"><span data-stu-id="7ac49-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7ac49-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ac49-122">Authorization</span></span>|<span data-ttu-id="7ac49-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="7ac49-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7ac49-124">承諾</span><span class="sxs-lookup"><span data-stu-id="7ac49-124">Accept</span></span>|<span data-ttu-id="7ac49-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7ac49-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ac49-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="7ac49-126">Request body</span></span>
<span data-ttu-id="7ac49-127">要求本文で、[windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7ac49-127">In the request body, supply a JSON representation for the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

<span data-ttu-id="7ac49-128">次の表に、[windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="7ac49-128">The following table shows the properties that are required when you create the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span></span>

|<span data-ttu-id="7ac49-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7ac49-129">Property</span></span>|<span data-ttu-id="7ac49-130">型</span><span class="sxs-lookup"><span data-stu-id="7ac49-130">Type</span></span>|<span data-ttu-id="7ac49-131">説明</span><span class="sxs-lookup"><span data-stu-id="7ac49-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ac49-132">id</span><span class="sxs-lookup"><span data-stu-id="7ac49-132">id</span></span>|<span data-ttu-id="7ac49-133">String</span><span class="sxs-lookup"><span data-stu-id="7ac49-133">String</span></span>|<span data-ttu-id="7ac49-134">WindowsInformationProtectionNetworkLearningSummary の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="7ac49-134">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="7ac49-135">url</span><span class="sxs-lookup"><span data-stu-id="7ac49-135">url</span></span>|<span data-ttu-id="7ac49-136">String</span><span class="sxs-lookup"><span data-stu-id="7ac49-136">String</span></span>|<span data-ttu-id="7ac49-137">Web サイト URL</span><span class="sxs-lookup"><span data-stu-id="7ac49-137">Website url</span></span>|
|<span data-ttu-id="7ac49-138">deviceCount</span><span class="sxs-lookup"><span data-stu-id="7ac49-138">deviceCount</span></span>|<span data-ttu-id="7ac49-139">Int32</span><span class="sxs-lookup"><span data-stu-id="7ac49-139">Int32</span></span>|<span data-ttu-id="7ac49-140">デバイス数</span><span class="sxs-lookup"><span data-stu-id="7ac49-140">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="7ac49-141">応答</span><span class="sxs-lookup"><span data-stu-id="7ac49-141">Response</span></span>
<span data-ttu-id="7ac49-142">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7ac49-142">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ac49-143">例</span><span class="sxs-lookup"><span data-stu-id="7ac49-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="7ac49-144">要求</span><span class="sxs-lookup"><span data-stu-id="7ac49-144">Request</span></span>
<span data-ttu-id="7ac49-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7ac49-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7ac49-146">応答</span><span class="sxs-lookup"><span data-stu-id="7ac49-146">Response</span></span>
<span data-ttu-id="7ac49-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7ac49-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




