---
title: windowsInformationProtectionNetworkLearningSummary の作成
description: 新しい windowsInformationProtectionNetworkLearningSummary オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 02a38617e2c47bd023ee4044126d0f4cf5308a8a
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30959951"
---
# <a name="create-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="feed4-103">windowsInformationProtectionNetworkLearningSummary の作成</span><span class="sxs-lookup"><span data-stu-id="feed4-103">Create windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="feed4-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="feed4-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="feed4-105">新しい [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="feed4-105">Create a new [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="feed4-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="feed4-106">Prerequisites</span></span>
<span data-ttu-id="feed4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="feed4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="feed4-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="feed4-109">Permission type</span></span>|<span data-ttu-id="feed4-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="feed4-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="feed4-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="feed4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="feed4-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="feed4-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="feed4-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="feed4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="feed4-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="feed4-114">Not supported.</span></span>|
|<span data-ttu-id="feed4-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="feed4-115">Application</span></span>|<span data-ttu-id="feed4-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="feed4-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="feed4-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="feed4-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionNetworkLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="feed4-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="feed4-118">Request headers</span></span>
|<span data-ttu-id="feed4-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="feed4-119">Header</span></span>|<span data-ttu-id="feed4-120">値</span><span class="sxs-lookup"><span data-stu-id="feed4-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="feed4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="feed4-121">Authorization</span></span>|<span data-ttu-id="feed4-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="feed4-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="feed4-123">承諾</span><span class="sxs-lookup"><span data-stu-id="feed4-123">Accept</span></span>|<span data-ttu-id="feed4-124">application/json</span><span class="sxs-lookup"><span data-stu-id="feed4-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="feed4-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="feed4-125">Request body</span></span>
<span data-ttu-id="feed4-126">要求本文で、windowsInformationProtectionNetworkLearningSummary オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="feed4-126">In the request body, supply a JSON representation for the windowsInformationProtectionNetworkLearningSummary object.</span></span>

<span data-ttu-id="feed4-127">次の表に、windowsInformationProtectionNetworkLearningSummary の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="feed4-127">The following table shows the properties that are required when you create the windowsInformationProtectionNetworkLearningSummary.</span></span>

|<span data-ttu-id="feed4-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="feed4-128">Property</span></span>|<span data-ttu-id="feed4-129">型</span><span class="sxs-lookup"><span data-stu-id="feed4-129">Type</span></span>|<span data-ttu-id="feed4-130">説明</span><span class="sxs-lookup"><span data-stu-id="feed4-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="feed4-131">id</span><span class="sxs-lookup"><span data-stu-id="feed4-131">id</span></span>|<span data-ttu-id="feed4-132">String</span><span class="sxs-lookup"><span data-stu-id="feed4-132">String</span></span>|<span data-ttu-id="feed4-133">WindowsInformationProtectionNetworkLearningSummary の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="feed4-133">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="feed4-134">url</span><span class="sxs-lookup"><span data-stu-id="feed4-134">url</span></span>|<span data-ttu-id="feed4-135">String</span><span class="sxs-lookup"><span data-stu-id="feed4-135">String</span></span>|<span data-ttu-id="feed4-136">Web サイト URL</span><span class="sxs-lookup"><span data-stu-id="feed4-136">Website url</span></span>|
|<span data-ttu-id="feed4-137">deviceCount</span><span class="sxs-lookup"><span data-stu-id="feed4-137">deviceCount</span></span>|<span data-ttu-id="feed4-138">Int32</span><span class="sxs-lookup"><span data-stu-id="feed4-138">Int32</span></span>|<span data-ttu-id="feed4-139">デバイス数</span><span class="sxs-lookup"><span data-stu-id="feed4-139">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="feed4-140">応答</span><span class="sxs-lookup"><span data-stu-id="feed4-140">Response</span></span>
<span data-ttu-id="feed4-141">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="feed4-141">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="feed4-142">例</span><span class="sxs-lookup"><span data-stu-id="feed4-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="feed4-143">要求</span><span class="sxs-lookup"><span data-stu-id="feed4-143">Request</span></span>
<span data-ttu-id="feed4-144">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="feed4-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionNetworkLearningSummaries
Content-type: application/json
Content-length: 137

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "url": "Url value",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="feed4-145">応答</span><span class="sxs-lookup"><span data-stu-id="feed4-145">Response</span></span>
<span data-ttu-id="feed4-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="feed4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 186

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "id": "242108f7-08f7-2421-f708-2124f7082124",
  "url": "Url value",
  "deviceCount": 11
}
```



