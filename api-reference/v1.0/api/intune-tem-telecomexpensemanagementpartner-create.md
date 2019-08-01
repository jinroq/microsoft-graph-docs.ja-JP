---
title: telecomExpenseManagementPartner の作成
description: 新しい telecomExpenseManagementPartner オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 58399603c12c7560dc1707b3c4badcee6700d6cb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36023377"
---
# <a name="create-telecomexpensemanagementpartner"></a><span data-ttu-id="18541-103">telecomExpenseManagementPartner の作成</span><span class="sxs-lookup"><span data-stu-id="18541-103">Create telecomExpenseManagementPartner</span></span>

> <span data-ttu-id="18541-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="18541-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18541-105">新しい [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="18541-105">Create a new [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="18541-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="18541-106">Prerequisites</span></span>
<span data-ttu-id="18541-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="18541-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18541-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="18541-109">Permission type</span></span>|<span data-ttu-id="18541-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="18541-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18541-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="18541-111">Delegated (work or school account)</span></span>|<span data-ttu-id="18541-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18541-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="18541-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="18541-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18541-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="18541-114">Not supported.</span></span>|
|<span data-ttu-id="18541-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="18541-115">Application</span></span>|<span data-ttu-id="18541-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="18541-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="18541-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="18541-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/telecomExpenseManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="18541-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="18541-118">Request headers</span></span>
|<span data-ttu-id="18541-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="18541-119">Header</span></span>|<span data-ttu-id="18541-120">値</span><span class="sxs-lookup"><span data-stu-id="18541-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18541-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="18541-121">Authorization</span></span>|<span data-ttu-id="18541-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="18541-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18541-123">承諾</span><span class="sxs-lookup"><span data-stu-id="18541-123">Accept</span></span>|<span data-ttu-id="18541-124">application/json</span><span class="sxs-lookup"><span data-stu-id="18541-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18541-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="18541-125">Request body</span></span>
<span data-ttu-id="18541-126">要求本文で、telecomExpenseManagementPartner オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="18541-126">In the request body, supply a JSON representation for the telecomExpenseManagementPartner object.</span></span>

<span data-ttu-id="18541-127">次の表に、telecomExpenseManagementPartner の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="18541-127">The following table shows the properties that are required when you create the telecomExpenseManagementPartner.</span></span>

|<span data-ttu-id="18541-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="18541-128">Property</span></span>|<span data-ttu-id="18541-129">型</span><span class="sxs-lookup"><span data-stu-id="18541-129">Type</span></span>|<span data-ttu-id="18541-130">説明</span><span class="sxs-lookup"><span data-stu-id="18541-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18541-131">id</span><span class="sxs-lookup"><span data-stu-id="18541-131">id</span></span>|<span data-ttu-id="18541-132">文字列</span><span class="sxs-lookup"><span data-stu-id="18541-132">String</span></span>|<span data-ttu-id="18541-133">TEM パートナーの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="18541-133">Unique identifier of the TEM partner.</span></span>|
|<span data-ttu-id="18541-134">displayName</span><span class="sxs-lookup"><span data-stu-id="18541-134">displayName</span></span>|<span data-ttu-id="18541-135">String</span><span class="sxs-lookup"><span data-stu-id="18541-135">String</span></span>|<span data-ttu-id="18541-136">TEM パートナーの表示名。</span><span class="sxs-lookup"><span data-stu-id="18541-136">Display name of the TEM partner.</span></span>|
|<span data-ttu-id="18541-137">url</span><span class="sxs-lookup"><span data-stu-id="18541-137">url</span></span>|<span data-ttu-id="18541-138">String</span><span class="sxs-lookup"><span data-stu-id="18541-138">String</span></span>|<span data-ttu-id="18541-139">TEM パートナーの管理用コントロール パネルの URL。管理者は、このパネルで TEM サービスを構成できます。</span><span class="sxs-lookup"><span data-stu-id="18541-139">URL of the TEM partner's administrative control panel, where an administrator can configure their TEM service.</span></span>|
|<span data-ttu-id="18541-140">appAuthorized</span><span class="sxs-lookup"><span data-stu-id="18541-140">appAuthorized</span></span>|<span data-ttu-id="18541-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="18541-141">Boolean</span></span>|<span data-ttu-id="18541-142">パートナーの AAD アプリに Intune へのアクセスが承認されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="18541-142">Whether the partner's AAD app has been authorized to access Intune.</span></span>|
|<span data-ttu-id="18541-143">enabled</span><span class="sxs-lookup"><span data-stu-id="18541-143">enabled</span></span>|<span data-ttu-id="18541-144">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="18541-144">Boolean</span></span>|<span data-ttu-id="18541-145">TEM サービスへの Intune の接続が現在有効であるか、無効であるかを示します。</span><span class="sxs-lookup"><span data-stu-id="18541-145">Whether Intune's connection to the TEM service is currently enabled or disabled.</span></span>|
|<span data-ttu-id="18541-146">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="18541-146">lastConnectionDateTime</span></span>|<span data-ttu-id="18541-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18541-147">DateTimeOffset</span></span>|<span data-ttu-id="18541-148">TEM パートナーによって Intune に最後に送信された要求のタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="18541-148">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="18541-149">応答</span><span class="sxs-lookup"><span data-stu-id="18541-149">Response</span></span>
<span data-ttu-id="18541-150">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="18541-150">If successful, this method returns a `201 Created` response code and a [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18541-151">例</span><span class="sxs-lookup"><span data-stu-id="18541-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="18541-152">要求</span><span class="sxs-lookup"><span data-stu-id="18541-152">Request</span></span>
<span data-ttu-id="18541-153">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="18541-153">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/telecomExpenseManagementPartners
Content-type: application/json
Content-length: 248

{
  "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
  "displayName": "Display Name value",
  "url": "Url value",
  "appAuthorized": true,
  "enabled": true,
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```

### <a name="response"></a><span data-ttu-id="18541-154">応答</span><span class="sxs-lookup"><span data-stu-id="18541-154">Response</span></span>
<span data-ttu-id="18541-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="18541-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



