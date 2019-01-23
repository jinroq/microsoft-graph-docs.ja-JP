---
title: windowsInformationProtectionAppLearningSummary の作成
description: 新しい windowsInformationProtectionAppLearningSummary オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3c39303154cbf09d6aedb1080d0560885e91133e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407761"
---
# <a name="create-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="b1578-103">windowsInformationProtectionAppLearningSummary の作成</span><span class="sxs-lookup"><span data-stu-id="b1578-103">Create windowsInformationProtectionAppLearningSummary</span></span>

> <span data-ttu-id="b1578-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b1578-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b1578-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b1578-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b1578-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b1578-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1578-107">新しい [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="b1578-107">Create a new [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b1578-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="b1578-108">Prerequisites</span></span>
<span data-ttu-id="b1578-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b1578-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b1578-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b1578-111">Permission type</span></span>|<span data-ttu-id="b1578-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b1578-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1578-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b1578-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b1578-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1578-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b1578-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b1578-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1578-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b1578-116">Not supported.</span></span>|
|<span data-ttu-id="b1578-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b1578-117">Application</span></span>|<span data-ttu-id="b1578-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b1578-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1578-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b1578-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionAppLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="b1578-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b1578-120">Request headers</span></span>
|<span data-ttu-id="b1578-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b1578-121">Header</span></span>|<span data-ttu-id="b1578-122">値</span><span class="sxs-lookup"><span data-stu-id="b1578-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b1578-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1578-123">Authorization</span></span>|<span data-ttu-id="b1578-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="b1578-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b1578-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b1578-125">Accept</span></span>|<span data-ttu-id="b1578-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b1578-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1578-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="b1578-127">Request body</span></span>
<span data-ttu-id="b1578-128">要求本文で、windowsInformationProtectionAppLearningSummary オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b1578-128">In the request body, supply a JSON representation for the windowsInformationProtectionAppLearningSummary object.</span></span>

<span data-ttu-id="b1578-129">次の表に、windowsInformationProtectionAppLearningSummary の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b1578-129">The following table shows the properties that are required when you create the windowsInformationProtectionAppLearningSummary.</span></span>

|<span data-ttu-id="b1578-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b1578-130">Property</span></span>|<span data-ttu-id="b1578-131">型</span><span class="sxs-lookup"><span data-stu-id="b1578-131">Type</span></span>|<span data-ttu-id="b1578-132">説明</span><span class="sxs-lookup"><span data-stu-id="b1578-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1578-133">id</span><span class="sxs-lookup"><span data-stu-id="b1578-133">id</span></span>|<span data-ttu-id="b1578-134">String</span><span class="sxs-lookup"><span data-stu-id="b1578-134">String</span></span>|<span data-ttu-id="b1578-135">WindowsInformationProtectionAppLearningSummary の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="b1578-135">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="b1578-136">applicationName</span><span class="sxs-lookup"><span data-stu-id="b1578-136">applicationName</span></span>|<span data-ttu-id="b1578-137">String</span><span class="sxs-lookup"><span data-stu-id="b1578-137">String</span></span>|<span data-ttu-id="b1578-138">アプリケーション名</span><span class="sxs-lookup"><span data-stu-id="b1578-138">Application Name</span></span>|
|<span data-ttu-id="b1578-139">applicationType</span><span class="sxs-lookup"><span data-stu-id="b1578-139">applicationType</span></span>|[<span data-ttu-id="b1578-140">applicationType</span><span class="sxs-lookup"><span data-stu-id="b1578-140">applicationType</span></span>](../resources/intune-wip-applicationtype.md)|<span data-ttu-id="b1578-141">アプリケーションの種類。</span><span class="sxs-lookup"><span data-stu-id="b1578-141">Application Type.</span></span> <span data-ttu-id="b1578-142">使用可能な値は、`universal`、`desktop` です。</span><span class="sxs-lookup"><span data-stu-id="b1578-142">Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="b1578-143">deviceCount</span><span class="sxs-lookup"><span data-stu-id="b1578-143">deviceCount</span></span>|<span data-ttu-id="b1578-144">Int32</span><span class="sxs-lookup"><span data-stu-id="b1578-144">Int32</span></span>|<span data-ttu-id="b1578-145">デバイス数</span><span class="sxs-lookup"><span data-stu-id="b1578-145">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="b1578-146">応答</span><span class="sxs-lookup"><span data-stu-id="b1578-146">Response</span></span>
<span data-ttu-id="b1578-147">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b1578-147">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1578-148">例</span><span class="sxs-lookup"><span data-stu-id="b1578-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="b1578-149">要求</span><span class="sxs-lookup"><span data-stu-id="b1578-149">Request</span></span>
<span data-ttu-id="b1578-150">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b1578-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsInformationProtectionAppLearningSummaries
Content-type: application/json
Content-length: 191

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "applicationName": "Application Name value",
  "applicationType": "desktop",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="b1578-151">応答</span><span class="sxs-lookup"><span data-stu-id="b1578-151">Response</span></span>
<span data-ttu-id="b1578-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b1578-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




