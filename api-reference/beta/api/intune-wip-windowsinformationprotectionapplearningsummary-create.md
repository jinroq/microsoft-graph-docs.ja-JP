---
title: windowsInformationProtectionAppLearningSummary の作成
description: 新しい windowsInformationProtectionAppLearningSummary オブジェクトを作成します。
ms.openlocfilehash: 671ab1efd631541871623fd1687639dd3d8d95ef
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073367"
---
# <a name="create-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="cc3fc-103">windowsInformationProtectionAppLearningSummary の作成</span><span class="sxs-lookup"><span data-stu-id="cc3fc-103">Create windowsInformationProtectionAppLearningSummary</span></span>

> <span data-ttu-id="cc3fc-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="cc3fc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cc3fc-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cc3fc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cc3fc-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="cc3fc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cc3fc-107">新しい [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="cc3fc-107">Create a new [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cc3fc-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="cc3fc-108">Prerequisites</span></span>
<span data-ttu-id="cc3fc-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cc3fc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc3fc-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cc3fc-111">Permission type</span></span>|<span data-ttu-id="cc3fc-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="cc3fc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cc3fc-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cc3fc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cc3fc-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc3fc-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cc3fc-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cc3fc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cc3fc-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cc3fc-116">Not supported.</span></span>|
|<span data-ttu-id="cc3fc-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cc3fc-117">Application</span></span>|<span data-ttu-id="cc3fc-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cc3fc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cc3fc-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cc3fc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionAppLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="cc3fc-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cc3fc-120">Request headers</span></span>
|<span data-ttu-id="cc3fc-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cc3fc-121">Header</span></span>|<span data-ttu-id="cc3fc-122">値</span><span class="sxs-lookup"><span data-stu-id="cc3fc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cc3fc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cc3fc-123">Authorization</span></span>|<span data-ttu-id="cc3fc-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="cc3fc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cc3fc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cc3fc-125">Accept</span></span>|<span data-ttu-id="cc3fc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cc3fc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cc3fc-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="cc3fc-127">Request body</span></span>
<span data-ttu-id="cc3fc-128">要求本文で、windowsInformationProtectionAppLearningSummary オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="cc3fc-128">In the request body, supply a JSON representation for the windowsInformationProtectionAppLearningSummary object.</span></span>

<span data-ttu-id="cc3fc-129">次の表に、windowsInformationProtectionAppLearningSummary の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="cc3fc-129">The following table shows the properties that are required when you create the windowsInformationProtectionAppLearningSummary.</span></span>

|<span data-ttu-id="cc3fc-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cc3fc-130">Property</span></span>|<span data-ttu-id="cc3fc-131">型</span><span class="sxs-lookup"><span data-stu-id="cc3fc-131">Type</span></span>|<span data-ttu-id="cc3fc-132">説明</span><span class="sxs-lookup"><span data-stu-id="cc3fc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc3fc-133">id</span><span class="sxs-lookup"><span data-stu-id="cc3fc-133">id</span></span>|<span data-ttu-id="cc3fc-134">String</span><span class="sxs-lookup"><span data-stu-id="cc3fc-134">String</span></span>|<span data-ttu-id="cc3fc-135">WindowsInformationProtectionAppLearningSummary の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="cc3fc-135">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="cc3fc-136">applicationName</span><span class="sxs-lookup"><span data-stu-id="cc3fc-136">applicationName</span></span>|<span data-ttu-id="cc3fc-137">String</span><span class="sxs-lookup"><span data-stu-id="cc3fc-137">String</span></span>|<span data-ttu-id="cc3fc-138">アプリケーション名</span><span class="sxs-lookup"><span data-stu-id="cc3fc-138">Application Name</span></span>|
|<span data-ttu-id="cc3fc-139">applicationType</span><span class="sxs-lookup"><span data-stu-id="cc3fc-139">applicationType</span></span>|[<span data-ttu-id="cc3fc-140">applicationType</span><span class="sxs-lookup"><span data-stu-id="cc3fc-140">applicationType</span></span>](../resources/intune-wip-applicationtype.md)|<span data-ttu-id="cc3fc-141">アプリケーションの種類。</span><span class="sxs-lookup"><span data-stu-id="cc3fc-141">Application Type.</span></span> <span data-ttu-id="cc3fc-142">使用可能な値は、`universal`、`desktop` です。</span><span class="sxs-lookup"><span data-stu-id="cc3fc-142">Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="cc3fc-143">deviceCount</span><span class="sxs-lookup"><span data-stu-id="cc3fc-143">deviceCount</span></span>|<span data-ttu-id="cc3fc-144">Int32</span><span class="sxs-lookup"><span data-stu-id="cc3fc-144">Int32</span></span>|<span data-ttu-id="cc3fc-145">デバイス数</span><span class="sxs-lookup"><span data-stu-id="cc3fc-145">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="cc3fc-146">応答</span><span class="sxs-lookup"><span data-stu-id="cc3fc-146">Response</span></span>
<span data-ttu-id="cc3fc-147">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="cc3fc-147">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc3fc-148">例</span><span class="sxs-lookup"><span data-stu-id="cc3fc-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="cc3fc-149">要求</span><span class="sxs-lookup"><span data-stu-id="cc3fc-149">Request</span></span>
<span data-ttu-id="cc3fc-150">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cc3fc-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cc3fc-151">応答</span><span class="sxs-lookup"><span data-stu-id="cc3fc-151">Response</span></span>
<span data-ttu-id="cc3fc-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cc3fc-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




