---
title: remoteAssistancePartner の作成
description: 新しい remoteAssistancePartner オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: 213898c6778b1700a2a3379bb8cd24689b5e671f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331109"
---
# <a name="create-remoteassistancepartner"></a><span data-ttu-id="04ce5-103">remoteAssistancePartner の作成</span><span class="sxs-lookup"><span data-stu-id="04ce5-103">Create remoteAssistancePartner</span></span>

> <span data-ttu-id="04ce5-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="04ce5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="04ce5-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="04ce5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="04ce5-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="04ce5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="04ce5-107">新しい [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="04ce5-107">Create a new [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="04ce5-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="04ce5-108">Prerequisites</span></span>
<span data-ttu-id="04ce5-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="04ce5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04ce5-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="04ce5-111">Permission type</span></span>|<span data-ttu-id="04ce5-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="04ce5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04ce5-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="04ce5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="04ce5-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04ce5-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="04ce5-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="04ce5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04ce5-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="04ce5-116">Not supported.</span></span>|
|<span data-ttu-id="04ce5-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="04ce5-117">Application</span></span>|<span data-ttu-id="04ce5-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="04ce5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="04ce5-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="04ce5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteAssistancePartners
```

## <a name="request-headers"></a><span data-ttu-id="04ce5-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="04ce5-120">Request headers</span></span>
|<span data-ttu-id="04ce5-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="04ce5-121">Header</span></span>|<span data-ttu-id="04ce5-122">値</span><span class="sxs-lookup"><span data-stu-id="04ce5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04ce5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="04ce5-123">Authorization</span></span>|<span data-ttu-id="04ce5-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="04ce5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04ce5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="04ce5-125">Accept</span></span>|<span data-ttu-id="04ce5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="04ce5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04ce5-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="04ce5-127">Request body</span></span>
<span data-ttu-id="04ce5-128">要求本文で、remoteAssistancePartner オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="04ce5-128">In the request body, supply a JSON representation for the remoteAssistancePartner object.</span></span>

<span data-ttu-id="04ce5-129">次の表に、remoteAssistancePartner の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="04ce5-129">The following table shows the properties that are required when you create the remoteAssistancePartner.</span></span>

|<span data-ttu-id="04ce5-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="04ce5-130">Property</span></span>|<span data-ttu-id="04ce5-131">種類</span><span class="sxs-lookup"><span data-stu-id="04ce5-131">Type</span></span>|<span data-ttu-id="04ce5-132">説明</span><span class="sxs-lookup"><span data-stu-id="04ce5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04ce5-133">ID</span><span class="sxs-lookup"><span data-stu-id="04ce5-133">id</span></span>|<span data-ttu-id="04ce5-134">String</span><span class="sxs-lookup"><span data-stu-id="04ce5-134">String</span></span>|<span data-ttu-id="04ce5-135">パートナーの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="04ce5-135">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="04ce5-136">displayName</span><span class="sxs-lookup"><span data-stu-id="04ce5-136">displayName</span></span>|<span data-ttu-id="04ce5-137">String</span><span class="sxs-lookup"><span data-stu-id="04ce5-137">String</span></span>|<span data-ttu-id="04ce5-138">パートナーの表示名。</span><span class="sxs-lookup"><span data-stu-id="04ce5-138">Display name of the partner.</span></span>|
|<span data-ttu-id="04ce5-139">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="04ce5-139">onboardingUrl</span></span>|<span data-ttu-id="04ce5-140">String</span><span class="sxs-lookup"><span data-stu-id="04ce5-140">String</span></span>|<span data-ttu-id="04ce5-141">パートナーのオンボーディング ポータルの URL。このポータルでは、管理者がパートナーのリモート アシスタンス サービスを構成できます。</span><span class="sxs-lookup"><span data-stu-id="04ce5-141">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="04ce5-142">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="04ce5-142">onboardingStatus</span></span>|[<span data-ttu-id="04ce5-143">remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="04ce5-143">remoteAssistanceOnboardingStatus</span></span>](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|<span data-ttu-id="04ce5-144">未定です。</span><span class="sxs-lookup"><span data-stu-id="04ce5-144">TBD.</span></span> <span data-ttu-id="04ce5-145">可能な値は、`notOnboarded`、`onboarding`、`onboarded` です。</span><span class="sxs-lookup"><span data-stu-id="04ce5-145">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="04ce5-146">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="04ce5-146">lastConnectionDateTime</span></span>|<span data-ttu-id="04ce5-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="04ce5-147">DateTimeOffset</span></span>|<span data-ttu-id="04ce5-148">TEM パートナーによって Intune に最後に送信された要求のタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="04ce5-148">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="04ce5-149">応答</span><span class="sxs-lookup"><span data-stu-id="04ce5-149">Response</span></span>
<span data-ttu-id="04ce5-150">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="04ce5-150">If successful, this method returns a `201 Created` response code and a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04ce5-151">例</span><span class="sxs-lookup"><span data-stu-id="04ce5-151">Example</span></span>
### <a name="request"></a><span data-ttu-id="04ce5-152">要求</span><span class="sxs-lookup"><span data-stu-id="04ce5-152">Request</span></span>
<span data-ttu-id="04ce5-153">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="04ce5-153">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/remoteAssistancePartners
Content-type: application/json
Content-length: 266

{
  "@odata.type": "#microsoft.graph.remoteAssistancePartner",
  "displayName": "Display Name value",
  "onboardingUrl": "https://example.com/onboardingUrl/",
  "onboardingStatus": "onboarding",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```

### <a name="response"></a><span data-ttu-id="04ce5-154">応答</span><span class="sxs-lookup"><span data-stu-id="04ce5-154">Response</span></span>
<span data-ttu-id="04ce5-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="04ce5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





