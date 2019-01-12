---
title: windowsInformationProtectionAppLearningSummary の作成
description: 新しい windowsInformationProtectionAppLearningSummary オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 66658cdd601ec7ea1af60a29a9302ca100debfaf
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940583"
---
# <a name="create-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="71782-103">windowsInformationProtectionAppLearningSummary の作成</span><span class="sxs-lookup"><span data-stu-id="71782-103">Create windowsInformationProtectionAppLearningSummary</span></span>

> <span data-ttu-id="71782-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="71782-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="71782-105">新しい [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="71782-105">Create a new [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="71782-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="71782-106">Prerequisites</span></span>
<span data-ttu-id="71782-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="71782-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71782-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="71782-109">Permission type</span></span>|<span data-ttu-id="71782-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="71782-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71782-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="71782-111">Delegated (work or school account)</span></span>|<span data-ttu-id="71782-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71782-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="71782-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="71782-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71782-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="71782-114">Not supported.</span></span>|
|<span data-ttu-id="71782-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="71782-115">Application</span></span>|<span data-ttu-id="71782-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="71782-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="71782-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="71782-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionAppLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="71782-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="71782-118">Request headers</span></span>
|<span data-ttu-id="71782-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="71782-119">Header</span></span>|<span data-ttu-id="71782-120">値</span><span class="sxs-lookup"><span data-stu-id="71782-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71782-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="71782-121">Authorization</span></span>|<span data-ttu-id="71782-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="71782-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71782-123">Accept</span><span class="sxs-lookup"><span data-stu-id="71782-123">Accept</span></span>|<span data-ttu-id="71782-124">application/json</span><span class="sxs-lookup"><span data-stu-id="71782-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71782-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="71782-125">Request body</span></span>
<span data-ttu-id="71782-126">要求本文で、windowsInformationProtectionAppLearningSummary オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="71782-126">In the request body, supply a JSON representation for the windowsInformationProtectionAppLearningSummary object.</span></span>

<span data-ttu-id="71782-127">次の表に、windowsInformationProtectionAppLearningSummary の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="71782-127">The following table shows the properties that are required when you create the windowsInformationProtectionAppLearningSummary.</span></span>

|<span data-ttu-id="71782-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="71782-128">Property</span></span>|<span data-ttu-id="71782-129">型</span><span class="sxs-lookup"><span data-stu-id="71782-129">Type</span></span>|<span data-ttu-id="71782-130">説明</span><span class="sxs-lookup"><span data-stu-id="71782-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71782-131">ID</span><span class="sxs-lookup"><span data-stu-id="71782-131">id</span></span>|<span data-ttu-id="71782-132">String</span><span class="sxs-lookup"><span data-stu-id="71782-132">String</span></span>|<span data-ttu-id="71782-133">WindowsInformationProtectionAppLearningSummary の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="71782-133">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="71782-134">applicationName</span><span class="sxs-lookup"><span data-stu-id="71782-134">applicationName</span></span>|<span data-ttu-id="71782-135">String</span><span class="sxs-lookup"><span data-stu-id="71782-135">String</span></span>|<span data-ttu-id="71782-136">アプリケーション名</span><span class="sxs-lookup"><span data-stu-id="71782-136">Application Name</span></span>|
|<span data-ttu-id="71782-137">applicationType</span><span class="sxs-lookup"><span data-stu-id="71782-137">applicationType</span></span>|[<span data-ttu-id="71782-138">applicationType</span><span class="sxs-lookup"><span data-stu-id="71782-138">applicationType</span></span>](../resources/intune-wip-applicationtype.md)|<span data-ttu-id="71782-139">アプリケーションの種類。</span><span class="sxs-lookup"><span data-stu-id="71782-139">Application Type.</span></span> <span data-ttu-id="71782-140">使用可能な値は、`universal`、`desktop` です。</span><span class="sxs-lookup"><span data-stu-id="71782-140">Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="71782-141">deviceCount</span><span class="sxs-lookup"><span data-stu-id="71782-141">deviceCount</span></span>|<span data-ttu-id="71782-142">Int32</span><span class="sxs-lookup"><span data-stu-id="71782-142">Int32</span></span>|<span data-ttu-id="71782-143">デバイス数</span><span class="sxs-lookup"><span data-stu-id="71782-143">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="71782-144">応答</span><span class="sxs-lookup"><span data-stu-id="71782-144">Response</span></span>
<span data-ttu-id="71782-145">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="71782-145">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71782-146">例</span><span class="sxs-lookup"><span data-stu-id="71782-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="71782-147">要求</span><span class="sxs-lookup"><span data-stu-id="71782-147">Request</span></span>
<span data-ttu-id="71782-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="71782-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="71782-149">応答</span><span class="sxs-lookup"><span data-stu-id="71782-149">Response</span></span>
<span data-ttu-id="71782-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="71782-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



