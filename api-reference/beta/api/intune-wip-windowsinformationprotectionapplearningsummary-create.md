---
title: windowsInformationProtectionAppLearningSummary の作成
description: 新しい windowsInformationProtectionAppLearningSummary オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 165664c3977ede205c406da712d5a331ff9de7c7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174658"
---
# <a name="create-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="a6253-103">windowsInformationProtectionAppLearningSummary の作成</span><span class="sxs-lookup"><span data-stu-id="a6253-103">Create windowsInformationProtectionAppLearningSummary</span></span>

> <span data-ttu-id="a6253-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a6253-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a6253-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a6253-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6253-106">新しい [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="a6253-106">Create a new [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a6253-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="a6253-107">Prerequisites</span></span>
<span data-ttu-id="a6253-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a6253-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a6253-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a6253-110">Permission type</span></span>|<span data-ttu-id="a6253-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a6253-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6253-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a6253-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a6253-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6253-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a6253-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a6253-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6253-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a6253-115">Not supported.</span></span>|
|<span data-ttu-id="a6253-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a6253-116">Application</span></span>|<span data-ttu-id="a6253-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a6253-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6253-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a6253-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionAppLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="a6253-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a6253-119">Request headers</span></span>
|<span data-ttu-id="a6253-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a6253-120">Header</span></span>|<span data-ttu-id="a6253-121">値</span><span class="sxs-lookup"><span data-stu-id="a6253-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6253-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a6253-122">Authorization</span></span>|<span data-ttu-id="a6253-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="a6253-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6253-124">承諾</span><span class="sxs-lookup"><span data-stu-id="a6253-124">Accept</span></span>|<span data-ttu-id="a6253-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a6253-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6253-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="a6253-126">Request body</span></span>
<span data-ttu-id="a6253-127">要求本文で、windowsInformationProtectionAppLearningSummary オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a6253-127">In the request body, supply a JSON representation for the windowsInformationProtectionAppLearningSummary object.</span></span>

<span data-ttu-id="a6253-128">次の表に、windowsInformationProtectionAppLearningSummary の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="a6253-128">The following table shows the properties that are required when you create the windowsInformationProtectionAppLearningSummary.</span></span>

|<span data-ttu-id="a6253-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a6253-129">Property</span></span>|<span data-ttu-id="a6253-130">型</span><span class="sxs-lookup"><span data-stu-id="a6253-130">Type</span></span>|<span data-ttu-id="a6253-131">説明</span><span class="sxs-lookup"><span data-stu-id="a6253-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6253-132">id</span><span class="sxs-lookup"><span data-stu-id="a6253-132">id</span></span>|<span data-ttu-id="a6253-133">String</span><span class="sxs-lookup"><span data-stu-id="a6253-133">String</span></span>|<span data-ttu-id="a6253-134">WindowsInformationProtectionAppLearningSummary の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="a6253-134">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="a6253-135">applicationName</span><span class="sxs-lookup"><span data-stu-id="a6253-135">applicationName</span></span>|<span data-ttu-id="a6253-136">String</span><span class="sxs-lookup"><span data-stu-id="a6253-136">String</span></span>|<span data-ttu-id="a6253-137">アプリケーション名</span><span class="sxs-lookup"><span data-stu-id="a6253-137">Application Name</span></span>|
|<span data-ttu-id="a6253-138">applicationType</span><span class="sxs-lookup"><span data-stu-id="a6253-138">applicationType</span></span>|[<span data-ttu-id="a6253-139">applicationType</span><span class="sxs-lookup"><span data-stu-id="a6253-139">applicationType</span></span>](../resources/intune-wip-applicationtype.md)|<span data-ttu-id="a6253-140">アプリケーションの種類。</span><span class="sxs-lookup"><span data-stu-id="a6253-140">Application Type.</span></span> <span data-ttu-id="a6253-141">使用可能な値は、`universal`、`desktop` です。</span><span class="sxs-lookup"><span data-stu-id="a6253-141">Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="a6253-142">deviceCount</span><span class="sxs-lookup"><span data-stu-id="a6253-142">deviceCount</span></span>|<span data-ttu-id="a6253-143">Int32</span><span class="sxs-lookup"><span data-stu-id="a6253-143">Int32</span></span>|<span data-ttu-id="a6253-144">デバイス数</span><span class="sxs-lookup"><span data-stu-id="a6253-144">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="a6253-145">応答</span><span class="sxs-lookup"><span data-stu-id="a6253-145">Response</span></span>
<span data-ttu-id="a6253-146">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a6253-146">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6253-147">例</span><span class="sxs-lookup"><span data-stu-id="a6253-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="a6253-148">要求</span><span class="sxs-lookup"><span data-stu-id="a6253-148">Request</span></span>
<span data-ttu-id="a6253-149">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a6253-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a6253-150">応答</span><span class="sxs-lookup"><span data-stu-id="a6253-150">Response</span></span>
<span data-ttu-id="a6253-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a6253-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




