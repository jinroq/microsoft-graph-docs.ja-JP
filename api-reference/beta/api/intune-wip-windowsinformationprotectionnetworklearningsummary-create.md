---
title: windowsInformationProtectionNetworkLearningSummary の作成
description: 新しい windowsInformationProtectionNetworkLearningSummary オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 72dbe090e23db5a912887f99aaa3f72eb5e71485
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35979142"
---
# <a name="create-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="fed6f-103">windowsInformationProtectionNetworkLearningSummary の作成</span><span class="sxs-lookup"><span data-stu-id="fed6f-103">Create windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="fed6f-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fed6f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fed6f-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="fed6f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fed6f-106">新しい [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="fed6f-106">Create a new [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fed6f-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="fed6f-107">Prerequisites</span></span>
<span data-ttu-id="fed6f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fed6f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fed6f-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fed6f-110">Permission type</span></span>|<span data-ttu-id="fed6f-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="fed6f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fed6f-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fed6f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fed6f-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fed6f-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fed6f-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fed6f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fed6f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fed6f-115">Not supported.</span></span>|
|<span data-ttu-id="fed6f-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fed6f-116">Application</span></span>|<span data-ttu-id="fed6f-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fed6f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fed6f-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fed6f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionNetworkLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="fed6f-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fed6f-119">Request headers</span></span>
|<span data-ttu-id="fed6f-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fed6f-120">Header</span></span>|<span data-ttu-id="fed6f-121">値</span><span class="sxs-lookup"><span data-stu-id="fed6f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fed6f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fed6f-122">Authorization</span></span>|<span data-ttu-id="fed6f-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="fed6f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fed6f-124">承諾</span><span class="sxs-lookup"><span data-stu-id="fed6f-124">Accept</span></span>|<span data-ttu-id="fed6f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fed6f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fed6f-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="fed6f-126">Request body</span></span>
<span data-ttu-id="fed6f-127">要求本文で、windowsInformationProtectionNetworkLearningSummary オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="fed6f-127">In the request body, supply a JSON representation for the windowsInformationProtectionNetworkLearningSummary object.</span></span>

<span data-ttu-id="fed6f-128">次の表に、windowsInformationProtectionNetworkLearningSummary の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="fed6f-128">The following table shows the properties that are required when you create the windowsInformationProtectionNetworkLearningSummary.</span></span>

|<span data-ttu-id="fed6f-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fed6f-129">Property</span></span>|<span data-ttu-id="fed6f-130">型</span><span class="sxs-lookup"><span data-stu-id="fed6f-130">Type</span></span>|<span data-ttu-id="fed6f-131">説明</span><span class="sxs-lookup"><span data-stu-id="fed6f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fed6f-132">id</span><span class="sxs-lookup"><span data-stu-id="fed6f-132">id</span></span>|<span data-ttu-id="fed6f-133">String</span><span class="sxs-lookup"><span data-stu-id="fed6f-133">String</span></span>|<span data-ttu-id="fed6f-134">WindowsInformationProtectionNetworkLearningSummary の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="fed6f-134">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="fed6f-135">url</span><span class="sxs-lookup"><span data-stu-id="fed6f-135">url</span></span>|<span data-ttu-id="fed6f-136">String</span><span class="sxs-lookup"><span data-stu-id="fed6f-136">String</span></span>|<span data-ttu-id="fed6f-137">Web サイト URL</span><span class="sxs-lookup"><span data-stu-id="fed6f-137">Website url</span></span>|
|<span data-ttu-id="fed6f-138">deviceCount</span><span class="sxs-lookup"><span data-stu-id="fed6f-138">deviceCount</span></span>|<span data-ttu-id="fed6f-139">Int32</span><span class="sxs-lookup"><span data-stu-id="fed6f-139">Int32</span></span>|<span data-ttu-id="fed6f-140">デバイス数</span><span class="sxs-lookup"><span data-stu-id="fed6f-140">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="fed6f-141">応答</span><span class="sxs-lookup"><span data-stu-id="fed6f-141">Response</span></span>
<span data-ttu-id="fed6f-142">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="fed6f-142">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fed6f-143">例</span><span class="sxs-lookup"><span data-stu-id="fed6f-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="fed6f-144">要求</span><span class="sxs-lookup"><span data-stu-id="fed6f-144">Request</span></span>
<span data-ttu-id="fed6f-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fed6f-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsInformationProtectionNetworkLearningSummaries
Content-type: application/json
Content-length: 137

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "url": "Url value",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="fed6f-146">応答</span><span class="sxs-lookup"><span data-stu-id="fed6f-146">Response</span></span>
<span data-ttu-id="fed6f-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fed6f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





