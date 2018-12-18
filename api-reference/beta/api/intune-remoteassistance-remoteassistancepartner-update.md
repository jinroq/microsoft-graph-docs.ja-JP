---
title: remoteAssistancePartner の更新
description: remoteAssistancePartner オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 119e5ab22ccd779635b66c06479024a4fc3f1ea6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27317312"
---
# <a name="update-remoteassistancepartner"></a><span data-ttu-id="fb9ff-103">remoteAssistancePartner の更新</span><span class="sxs-lookup"><span data-stu-id="fb9ff-103">Update remoteAssistancePartner</span></span>

> <span data-ttu-id="fb9ff-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fb9ff-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fb9ff-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fb9ff-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fb9ff-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="fb9ff-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fb9ff-107">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="fb9ff-107">Update the properties of a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fb9ff-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="fb9ff-108">Prerequisites</span></span>
<span data-ttu-id="fb9ff-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fb9ff-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb9ff-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fb9ff-111">Permission type</span></span>|<span data-ttu-id="fb9ff-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="fb9ff-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb9ff-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fb9ff-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fb9ff-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb9ff-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="fb9ff-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fb9ff-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb9ff-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fb9ff-116">Not supported.</span></span>|
|<span data-ttu-id="fb9ff-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fb9ff-117">Application</span></span>|<span data-ttu-id="fb9ff-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fb9ff-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb9ff-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fb9ff-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="fb9ff-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fb9ff-120">Request headers</span></span>
|<span data-ttu-id="fb9ff-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fb9ff-121">Header</span></span>|<span data-ttu-id="fb9ff-122">値</span><span class="sxs-lookup"><span data-stu-id="fb9ff-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb9ff-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fb9ff-123">Authorization</span></span>|<span data-ttu-id="fb9ff-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="fb9ff-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fb9ff-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fb9ff-125">Accept</span></span>|<span data-ttu-id="fb9ff-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fb9ff-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb9ff-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="fb9ff-127">Request body</span></span>
<span data-ttu-id="fb9ff-128">要求本文で、[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="fb9ff-128">In the request body, supply a JSON representation for the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>

<span data-ttu-id="fb9ff-129">次の表に、[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="fb9ff-129">The following table shows the properties that are required when you create the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span></span>

|<span data-ttu-id="fb9ff-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fb9ff-130">Property</span></span>|<span data-ttu-id="fb9ff-131">種類</span><span class="sxs-lookup"><span data-stu-id="fb9ff-131">Type</span></span>|<span data-ttu-id="fb9ff-132">説明</span><span class="sxs-lookup"><span data-stu-id="fb9ff-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb9ff-133">ID</span><span class="sxs-lookup"><span data-stu-id="fb9ff-133">id</span></span>|<span data-ttu-id="fb9ff-134">String</span><span class="sxs-lookup"><span data-stu-id="fb9ff-134">String</span></span>|<span data-ttu-id="fb9ff-135">パートナーの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="fb9ff-135">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="fb9ff-136">displayName</span><span class="sxs-lookup"><span data-stu-id="fb9ff-136">displayName</span></span>|<span data-ttu-id="fb9ff-137">String</span><span class="sxs-lookup"><span data-stu-id="fb9ff-137">String</span></span>|<span data-ttu-id="fb9ff-138">パートナーの表示名。</span><span class="sxs-lookup"><span data-stu-id="fb9ff-138">Display name of the partner.</span></span>|
|<span data-ttu-id="fb9ff-139">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="fb9ff-139">onboardingUrl</span></span>|<span data-ttu-id="fb9ff-140">String</span><span class="sxs-lookup"><span data-stu-id="fb9ff-140">String</span></span>|<span data-ttu-id="fb9ff-141">パートナーのオンボーディング ポータルの URL。このポータルでは、管理者がパートナーのリモート アシスタンス サービスを構成できます。</span><span class="sxs-lookup"><span data-stu-id="fb9ff-141">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="fb9ff-142">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="fb9ff-142">onboardingStatus</span></span>|[<span data-ttu-id="fb9ff-143">remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="fb9ff-143">remoteAssistanceOnboardingStatus</span></span>](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|<span data-ttu-id="fb9ff-144">未定です。</span><span class="sxs-lookup"><span data-stu-id="fb9ff-144">TBD.</span></span> <span data-ttu-id="fb9ff-145">可能な値は、`notOnboarded`、`onboarding`、`onboarded` です。</span><span class="sxs-lookup"><span data-stu-id="fb9ff-145">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="fb9ff-146">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="fb9ff-146">lastConnectionDateTime</span></span>|<span data-ttu-id="fb9ff-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb9ff-147">DateTimeOffset</span></span>|<span data-ttu-id="fb9ff-148">TEM パートナーによって Intune に最後に送信された要求のタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="fb9ff-148">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="fb9ff-149">応答</span><span class="sxs-lookup"><span data-stu-id="fb9ff-149">Response</span></span>
<span data-ttu-id="fb9ff-150">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="fb9ff-150">If successful, this method returns a `200 OK` response code and an updated [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb9ff-151">例</span><span class="sxs-lookup"><span data-stu-id="fb9ff-151">Example</span></span>
### <a name="request"></a><span data-ttu-id="fb9ff-152">要求</span><span class="sxs-lookup"><span data-stu-id="fb9ff-152">Request</span></span>
<span data-ttu-id="fb9ff-153">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fb9ff-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
Content-type: application/json
Content-length: 204

{
  "displayName": "Display Name value",
  "onboardingUrl": "https://example.com/onboardingUrl/",
  "onboardingStatus": "onboarding",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```

### <a name="response"></a><span data-ttu-id="fb9ff-154">応答</span><span class="sxs-lookup"><span data-stu-id="fb9ff-154">Response</span></span>
<span data-ttu-id="fb9ff-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fb9ff-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 315

{
  "@odata.type": "#microsoft.graph.remoteAssistancePartner",
  "id": "7443c8b9-c8b9-7443-b9c8-4374b9c84374",
  "displayName": "Display Name value",
  "onboardingUrl": "https://example.com/onboardingUrl/",
  "onboardingStatus": "onboarding",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```





