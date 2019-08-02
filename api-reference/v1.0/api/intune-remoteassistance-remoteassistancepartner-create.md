---
title: remoteAssistancePartner の作成
description: 新しい remoteAssistancePartner オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7b0c3f59d3e5169444d782c139e954e87904defe
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36023658"
---
# <a name="create-remoteassistancepartner"></a><span data-ttu-id="31389-103">remoteAssistancePartner の作成</span><span class="sxs-lookup"><span data-stu-id="31389-103">Create remoteAssistancePartner</span></span>

> <span data-ttu-id="31389-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="31389-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="31389-105">新しい [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="31389-105">Create a new [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="31389-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="31389-106">Prerequisites</span></span>
<span data-ttu-id="31389-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="31389-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31389-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="31389-109">Permission type</span></span>|<span data-ttu-id="31389-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="31389-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="31389-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="31389-111">Delegated (work or school account)</span></span>|<span data-ttu-id="31389-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31389-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="31389-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="31389-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="31389-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="31389-114">Not supported.</span></span>|
|<span data-ttu-id="31389-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="31389-115">Application</span></span>|<span data-ttu-id="31389-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="31389-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="31389-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="31389-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteAssistancePartners
```

## <a name="request-headers"></a><span data-ttu-id="31389-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="31389-118">Request headers</span></span>
|<span data-ttu-id="31389-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="31389-119">Header</span></span>|<span data-ttu-id="31389-120">値</span><span class="sxs-lookup"><span data-stu-id="31389-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="31389-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="31389-121">Authorization</span></span>|<span data-ttu-id="31389-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="31389-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="31389-123">承諾</span><span class="sxs-lookup"><span data-stu-id="31389-123">Accept</span></span>|<span data-ttu-id="31389-124">application/json</span><span class="sxs-lookup"><span data-stu-id="31389-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="31389-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="31389-125">Request body</span></span>
<span data-ttu-id="31389-126">要求本文で、remoteAssistancePartner オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="31389-126">In the request body, supply a JSON representation for the remoteAssistancePartner object.</span></span>

<span data-ttu-id="31389-127">次の表に、remoteAssistancePartner の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="31389-127">The following table shows the properties that are required when you create the remoteAssistancePartner.</span></span>

|<span data-ttu-id="31389-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="31389-128">Property</span></span>|<span data-ttu-id="31389-129">型</span><span class="sxs-lookup"><span data-stu-id="31389-129">Type</span></span>|<span data-ttu-id="31389-130">説明</span><span class="sxs-lookup"><span data-stu-id="31389-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31389-131">id</span><span class="sxs-lookup"><span data-stu-id="31389-131">id</span></span>|<span data-ttu-id="31389-132">文字列</span><span class="sxs-lookup"><span data-stu-id="31389-132">String</span></span>|<span data-ttu-id="31389-133">パートナーの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="31389-133">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="31389-134">displayName</span><span class="sxs-lookup"><span data-stu-id="31389-134">displayName</span></span>|<span data-ttu-id="31389-135">String</span><span class="sxs-lookup"><span data-stu-id="31389-135">String</span></span>|<span data-ttu-id="31389-136">パートナーの表示名。</span><span class="sxs-lookup"><span data-stu-id="31389-136">Display name of the partner.</span></span>|
|<span data-ttu-id="31389-137">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="31389-137">onboardingUrl</span></span>|<span data-ttu-id="31389-138">String</span><span class="sxs-lookup"><span data-stu-id="31389-138">String</span></span>|<span data-ttu-id="31389-139">パートナーのオンボーディング ポータルの URL。このポータルでは、管理者がパートナーのリモート アシスタンス サービスを構成できます。</span><span class="sxs-lookup"><span data-stu-id="31389-139">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="31389-140">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="31389-140">onboardingStatus</span></span>|[<span data-ttu-id="31389-141">remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="31389-141">remoteAssistanceOnboardingStatus</span></span>](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|<span data-ttu-id="31389-142">TBD.</span><span class="sxs-lookup"><span data-stu-id="31389-142">TBD.</span></span> <span data-ttu-id="31389-143">可能な値は、`notOnboarded`、`onboarding`、`onboarded` です。</span><span class="sxs-lookup"><span data-stu-id="31389-143">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="31389-144">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="31389-144">lastConnectionDateTime</span></span>|<span data-ttu-id="31389-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31389-145">DateTimeOffset</span></span>|<span data-ttu-id="31389-146">TEM パートナーによって Intune に最後に送信された要求のタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="31389-146">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="31389-147">応答</span><span class="sxs-lookup"><span data-stu-id="31389-147">Response</span></span>
<span data-ttu-id="31389-148">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="31389-148">If successful, this method returns a `201 Created` response code and a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31389-149">例</span><span class="sxs-lookup"><span data-stu-id="31389-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="31389-150">要求</span><span class="sxs-lookup"><span data-stu-id="31389-150">Request</span></span>
<span data-ttu-id="31389-151">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="31389-151">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/remoteAssistancePartners
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

### <a name="response"></a><span data-ttu-id="31389-152">応答</span><span class="sxs-lookup"><span data-stu-id="31389-152">Response</span></span>
<span data-ttu-id="31389-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="31389-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



