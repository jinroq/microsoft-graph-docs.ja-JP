---
title: telecomExpenseManagementPartner の更新
description: telecomExpenseManagementPartner オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 5180ce7338bdffde0fb51f504882e2b82ca96cac
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27318726"
---
# <a name="update-telecomexpensemanagementpartner"></a><span data-ttu-id="092c7-103">telecomExpenseManagementPartner の更新</span><span class="sxs-lookup"><span data-stu-id="092c7-103">Update telecomExpenseManagementPartner</span></span>

> <span data-ttu-id="092c7-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="092c7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="092c7-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="092c7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="092c7-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="092c7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="092c7-107">[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="092c7-107">Update the properties of a [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="092c7-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="092c7-108">Prerequisites</span></span>
<span data-ttu-id="092c7-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="092c7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="092c7-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="092c7-111">Permission type</span></span>|<span data-ttu-id="092c7-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="092c7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="092c7-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="092c7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="092c7-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="092c7-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="092c7-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="092c7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="092c7-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="092c7-116">Not supported.</span></span>|
|<span data-ttu-id="092c7-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="092c7-117">Application</span></span>|<span data-ttu-id="092c7-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="092c7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="092c7-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="092c7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="092c7-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="092c7-120">Request headers</span></span>
|<span data-ttu-id="092c7-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="092c7-121">Header</span></span>|<span data-ttu-id="092c7-122">値</span><span class="sxs-lookup"><span data-stu-id="092c7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="092c7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="092c7-123">Authorization</span></span>|<span data-ttu-id="092c7-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="092c7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="092c7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="092c7-125">Accept</span></span>|<span data-ttu-id="092c7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="092c7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="092c7-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="092c7-127">Request body</span></span>
<span data-ttu-id="092c7-128">要求本文で、[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="092c7-128">In the request body, supply a JSON representation for the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>

<span data-ttu-id="092c7-129">次の表に、[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="092c7-129">The following table shows the properties that are required when you create the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span></span>

|<span data-ttu-id="092c7-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="092c7-130">Property</span></span>|<span data-ttu-id="092c7-131">種類</span><span class="sxs-lookup"><span data-stu-id="092c7-131">Type</span></span>|<span data-ttu-id="092c7-132">説明</span><span class="sxs-lookup"><span data-stu-id="092c7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="092c7-133">ID</span><span class="sxs-lookup"><span data-stu-id="092c7-133">id</span></span>|<span data-ttu-id="092c7-134">String</span><span class="sxs-lookup"><span data-stu-id="092c7-134">String</span></span>|<span data-ttu-id="092c7-135">TEM パートナーの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="092c7-135">Unique identifier of the TEM partner.</span></span>|
|<span data-ttu-id="092c7-136">displayName</span><span class="sxs-lookup"><span data-stu-id="092c7-136">displayName</span></span>|<span data-ttu-id="092c7-137">String</span><span class="sxs-lookup"><span data-stu-id="092c7-137">String</span></span>|<span data-ttu-id="092c7-138">TEM パートナーの表示名。</span><span class="sxs-lookup"><span data-stu-id="092c7-138">Display name of the TEM partner.</span></span>|
|<span data-ttu-id="092c7-139">url</span><span class="sxs-lookup"><span data-stu-id="092c7-139">url</span></span>|<span data-ttu-id="092c7-140">String</span><span class="sxs-lookup"><span data-stu-id="092c7-140">String</span></span>|<span data-ttu-id="092c7-141">TEM パートナーの管理用コントロール パネルの URL。管理者はここで TEM サービスを構成できます。</span><span class="sxs-lookup"><span data-stu-id="092c7-141">URL of the TEM partner's administrative control panel, where an administrator can configure their TEM service.</span></span>|
|<span data-ttu-id="092c7-142">appAuthorized</span><span class="sxs-lookup"><span data-stu-id="092c7-142">appAuthorized</span></span>|<span data-ttu-id="092c7-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="092c7-143">Boolean</span></span>|<span data-ttu-id="092c7-144">パートナーの AAD アプリに Intune へのアクセスが承認されているかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="092c7-144">Whether the partner's AAD app has been authorized to access Intune.</span></span>|
|<span data-ttu-id="092c7-145">enabled</span><span class="sxs-lookup"><span data-stu-id="092c7-145">enabled</span></span>|<span data-ttu-id="092c7-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="092c7-146">Boolean</span></span>|<span data-ttu-id="092c7-147">TEM サービスへの Intune の接続が現在有効であるか、無効であるかを指定します。</span><span class="sxs-lookup"><span data-stu-id="092c7-147">Whether Intune's connection to the TEM service is currently enabled or disabled.</span></span>|
|<span data-ttu-id="092c7-148">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="092c7-148">lastConnectionDateTime</span></span>|<span data-ttu-id="092c7-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="092c7-149">DateTimeOffset</span></span>|<span data-ttu-id="092c7-150">TEM パートナーによって Intune に最後に送信された要求のタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="092c7-150">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="092c7-151">応答</span><span class="sxs-lookup"><span data-stu-id="092c7-151">Response</span></span>
<span data-ttu-id="092c7-152">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="092c7-152">If successful, this method returns a `200 OK` response code and an updated [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="092c7-153">例</span><span class="sxs-lookup"><span data-stu-id="092c7-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="092c7-154">要求</span><span class="sxs-lookup"><span data-stu-id="092c7-154">Request</span></span>
<span data-ttu-id="092c7-155">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="092c7-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
Content-type: application/json
Content-length: 178

{
  "displayName": "Display Name value",
  "url": "Url value",
  "appAuthorized": true,
  "enabled": true,
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```

### <a name="response"></a><span data-ttu-id="092c7-156">応答</span><span class="sxs-lookup"><span data-stu-id="092c7-156">Response</span></span>
<span data-ttu-id="092c7-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="092c7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 297

{
  "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
  "id": "47a3b399-b399-47a3-99b3-a34799b3a347",
  "displayName": "Display Name value",
  "url": "Url value",
  "appAuthorized": true,
  "enabled": true,
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```




