---
title: MicrosoftStoreForBusinessContainedApp を作成します。
description: 新しい microsoftStoreForBusinessContainedApp オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ac782261c00008bf9b4ab552932f8f841a9965bc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843296"
---
# <a name="create-microsoftstoreforbusinesscontainedapp"></a><span data-ttu-id="79ac6-103">MicrosoftStoreForBusinessContainedApp を作成します。</span><span class="sxs-lookup"><span data-stu-id="79ac6-103">Create microsoftStoreForBusinessContainedApp</span></span>

> <span data-ttu-id="79ac6-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="79ac6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="79ac6-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="79ac6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="79ac6-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="79ac6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="79ac6-107">新しい[microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="79ac6-107">Create a new [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="79ac6-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="79ac6-108">Prerequisites</span></span>
<span data-ttu-id="79ac6-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="79ac6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79ac6-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="79ac6-111">Permission type</span></span>|<span data-ttu-id="79ac6-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="79ac6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79ac6-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="79ac6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="79ac6-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79ac6-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="79ac6-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="79ac6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79ac6-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="79ac6-116">Not supported.</span></span>|
|<span data-ttu-id="79ac6-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="79ac6-117">Application</span></span>|<span data-ttu-id="79ac6-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="79ac6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="79ac6-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="79ac6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps
```

## <a name="request-headers"></a><span data-ttu-id="79ac6-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="79ac6-120">Request headers</span></span>
|<span data-ttu-id="79ac6-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="79ac6-121">Header</span></span>|<span data-ttu-id="79ac6-122">値</span><span class="sxs-lookup"><span data-stu-id="79ac6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79ac6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="79ac6-123">Authorization</span></span>|<span data-ttu-id="79ac6-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="79ac6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79ac6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="79ac6-125">Accept</span></span>|<span data-ttu-id="79ac6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="79ac6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79ac6-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="79ac6-127">Request body</span></span>
<span data-ttu-id="79ac6-128">要求の本文に microsoftStoreForBusinessContainedApp オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="79ac6-128">In the request body, supply a JSON representation for the microsoftStoreForBusinessContainedApp object.</span></span>

<span data-ttu-id="79ac6-129">次の表は、microsoftStoreForBusinessContainedApp を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="79ac6-129">The following table shows the properties that are required when you create the microsoftStoreForBusinessContainedApp.</span></span>

|<span data-ttu-id="79ac6-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="79ac6-130">Property</span></span>|<span data-ttu-id="79ac6-131">種類</span><span class="sxs-lookup"><span data-stu-id="79ac6-131">Type</span></span>|<span data-ttu-id="79ac6-132">説明</span><span class="sxs-lookup"><span data-stu-id="79ac6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79ac6-133">ID</span><span class="sxs-lookup"><span data-stu-id="79ac6-133">id</span></span>|<span data-ttu-id="79ac6-134">String</span><span class="sxs-lookup"><span data-stu-id="79ac6-134">String</span></span>|<span data-ttu-id="79ac6-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="79ac6-135">Key of the entity.</span></span> <span data-ttu-id="79ac6-136">[MobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="79ac6-136">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="79ac6-137">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="79ac6-137">appUserModelId</span></span>|<span data-ttu-id="79ac6-138">String</span><span class="sxs-lookup"><span data-stu-id="79ac6-138">String</span></span>|<span data-ttu-id="79ac6-139">MicrosoftStoreForBusinessApp の格納されているアプリケーションのアプリケーション ユーザー モデル ID です。</span><span class="sxs-lookup"><span data-stu-id="79ac6-139">The app user model ID of the contained app of a MicrosoftStoreForBusinessApp.</span></span>|



## <a name="response"></a><span data-ttu-id="79ac6-140">応答</span><span class="sxs-lookup"><span data-stu-id="79ac6-140">Response</span></span>
<span data-ttu-id="79ac6-141">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="79ac6-141">If successful, this method returns a `201 Created` response code and a [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79ac6-142">例</span><span class="sxs-lookup"><span data-stu-id="79ac6-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="79ac6-143">要求</span><span class="sxs-lookup"><span data-stu-id="79ac6-143">Request</span></span>
<span data-ttu-id="79ac6-144">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="79ac6-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
Content-type: application/json
Content-length: 127

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="79ac6-145">応答</span><span class="sxs-lookup"><span data-stu-id="79ac6-145">Response</span></span>
<span data-ttu-id="79ac6-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="79ac6-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 176

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessContainedApp",
  "id": "bf1d79df-79df-bf1d-df79-1dbfdf791dbf",
  "appUserModelId": "App User Model Id value"
}
```





