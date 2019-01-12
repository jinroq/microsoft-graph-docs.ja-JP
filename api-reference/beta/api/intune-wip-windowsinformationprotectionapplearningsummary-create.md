---
title: windowsInformationProtectionAppLearningSummary の作成
description: 新しい windowsInformationProtectionAppLearningSummary オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 70fd9c5649928fe7c6e91b38450010b70d973c58
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27944601"
---
# <a name="create-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="016f2-103">windowsInformationProtectionAppLearningSummary の作成</span><span class="sxs-lookup"><span data-stu-id="016f2-103">Create windowsInformationProtectionAppLearningSummary</span></span>

> <span data-ttu-id="016f2-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="016f2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="016f2-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="016f2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="016f2-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="016f2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="016f2-107">新しい [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="016f2-107">Create a new [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="016f2-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="016f2-108">Prerequisites</span></span>
<span data-ttu-id="016f2-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="016f2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="016f2-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="016f2-111">Permission type</span></span>|<span data-ttu-id="016f2-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="016f2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="016f2-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="016f2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="016f2-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="016f2-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="016f2-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="016f2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="016f2-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="016f2-116">Not supported.</span></span>|
|<span data-ttu-id="016f2-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="016f2-117">Application</span></span>|<span data-ttu-id="016f2-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="016f2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="016f2-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="016f2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionAppLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="016f2-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="016f2-120">Request headers</span></span>
|<span data-ttu-id="016f2-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="016f2-121">Header</span></span>|<span data-ttu-id="016f2-122">値</span><span class="sxs-lookup"><span data-stu-id="016f2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="016f2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="016f2-123">Authorization</span></span>|<span data-ttu-id="016f2-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="016f2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="016f2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="016f2-125">Accept</span></span>|<span data-ttu-id="016f2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="016f2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="016f2-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="016f2-127">Request body</span></span>
<span data-ttu-id="016f2-128">要求本文で、windowsInformationProtectionAppLearningSummary オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="016f2-128">In the request body, supply a JSON representation for the windowsInformationProtectionAppLearningSummary object.</span></span>

<span data-ttu-id="016f2-129">次の表に、windowsInformationProtectionAppLearningSummary の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="016f2-129">The following table shows the properties that are required when you create the windowsInformationProtectionAppLearningSummary.</span></span>

|<span data-ttu-id="016f2-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="016f2-130">Property</span></span>|<span data-ttu-id="016f2-131">型</span><span class="sxs-lookup"><span data-stu-id="016f2-131">Type</span></span>|<span data-ttu-id="016f2-132">説明</span><span class="sxs-lookup"><span data-stu-id="016f2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="016f2-133">ID</span><span class="sxs-lookup"><span data-stu-id="016f2-133">id</span></span>|<span data-ttu-id="016f2-134">String</span><span class="sxs-lookup"><span data-stu-id="016f2-134">String</span></span>|<span data-ttu-id="016f2-135">WindowsInformationProtectionAppLearningSummary の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="016f2-135">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="016f2-136">applicationName</span><span class="sxs-lookup"><span data-stu-id="016f2-136">applicationName</span></span>|<span data-ttu-id="016f2-137">String</span><span class="sxs-lookup"><span data-stu-id="016f2-137">String</span></span>|<span data-ttu-id="016f2-138">アプリケーション名</span><span class="sxs-lookup"><span data-stu-id="016f2-138">Application Name</span></span>|
|<span data-ttu-id="016f2-139">applicationType</span><span class="sxs-lookup"><span data-stu-id="016f2-139">applicationType</span></span>|[<span data-ttu-id="016f2-140">applicationType</span><span class="sxs-lookup"><span data-stu-id="016f2-140">applicationType</span></span>](../resources/intune-wip-applicationtype.md)|<span data-ttu-id="016f2-141">アプリケーションの種類。</span><span class="sxs-lookup"><span data-stu-id="016f2-141">Application Type.</span></span> <span data-ttu-id="016f2-142">使用可能な値は、`universal`、`desktop` です。</span><span class="sxs-lookup"><span data-stu-id="016f2-142">Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="016f2-143">deviceCount</span><span class="sxs-lookup"><span data-stu-id="016f2-143">deviceCount</span></span>|<span data-ttu-id="016f2-144">Int32</span><span class="sxs-lookup"><span data-stu-id="016f2-144">Int32</span></span>|<span data-ttu-id="016f2-145">デバイス数</span><span class="sxs-lookup"><span data-stu-id="016f2-145">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="016f2-146">応答</span><span class="sxs-lookup"><span data-stu-id="016f2-146">Response</span></span>
<span data-ttu-id="016f2-147">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="016f2-147">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="016f2-148">例</span><span class="sxs-lookup"><span data-stu-id="016f2-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="016f2-149">要求</span><span class="sxs-lookup"><span data-stu-id="016f2-149">Request</span></span>
<span data-ttu-id="016f2-150">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="016f2-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="016f2-151">応答</span><span class="sxs-lookup"><span data-stu-id="016f2-151">Response</span></span>
<span data-ttu-id="016f2-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="016f2-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





