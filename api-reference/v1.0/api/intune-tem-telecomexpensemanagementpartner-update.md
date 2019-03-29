---
title: telecomExpenseManagementPartner の更新
description: telecomExpenseManagementPartner オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1ca6b2dd0d55c1dc00395bdab44becb238c13f67
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30968099"
---
# <a name="update-telecomexpensemanagementpartner"></a><span data-ttu-id="270da-103">telecomExpenseManagementPartner の更新</span><span class="sxs-lookup"><span data-stu-id="270da-103">Update telecomExpenseManagementPartner</span></span>

> <span data-ttu-id="270da-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="270da-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="270da-105">[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="270da-105">Update the properties of a [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="270da-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="270da-106">Prerequisites</span></span>
<span data-ttu-id="270da-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="270da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="270da-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="270da-109">Permission type</span></span>|<span data-ttu-id="270da-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="270da-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="270da-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="270da-111">Delegated (work or school account)</span></span>|<span data-ttu-id="270da-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="270da-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="270da-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="270da-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="270da-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="270da-114">Not supported.</span></span>|
|<span data-ttu-id="270da-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="270da-115">Application</span></span>|<span data-ttu-id="270da-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="270da-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="270da-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="270da-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="270da-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="270da-118">Request headers</span></span>
|<span data-ttu-id="270da-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="270da-119">Header</span></span>|<span data-ttu-id="270da-120">値</span><span class="sxs-lookup"><span data-stu-id="270da-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="270da-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="270da-121">Authorization</span></span>|<span data-ttu-id="270da-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="270da-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="270da-123">承諾</span><span class="sxs-lookup"><span data-stu-id="270da-123">Accept</span></span>|<span data-ttu-id="270da-124">application/json</span><span class="sxs-lookup"><span data-stu-id="270da-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="270da-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="270da-125">Request body</span></span>
<span data-ttu-id="270da-126">要求本文で、[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="270da-126">In the request body, supply a JSON representation for the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>

<span data-ttu-id="270da-127">次の表に、[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="270da-127">The following table shows the properties that are required when you create the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span></span>

|<span data-ttu-id="270da-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="270da-128">Property</span></span>|<span data-ttu-id="270da-129">型</span><span class="sxs-lookup"><span data-stu-id="270da-129">Type</span></span>|<span data-ttu-id="270da-130">説明</span><span class="sxs-lookup"><span data-stu-id="270da-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="270da-131">id</span><span class="sxs-lookup"><span data-stu-id="270da-131">id</span></span>|<span data-ttu-id="270da-132">文字列</span><span class="sxs-lookup"><span data-stu-id="270da-132">String</span></span>|<span data-ttu-id="270da-133">TEM パートナーの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="270da-133">Unique identifier of the TEM partner.</span></span>|
|<span data-ttu-id="270da-134">displayName</span><span class="sxs-lookup"><span data-stu-id="270da-134">displayName</span></span>|<span data-ttu-id="270da-135">String</span><span class="sxs-lookup"><span data-stu-id="270da-135">String</span></span>|<span data-ttu-id="270da-136">TEM パートナーの表示名。</span><span class="sxs-lookup"><span data-stu-id="270da-136">Display name of the TEM partner.</span></span>|
|<span data-ttu-id="270da-137">url</span><span class="sxs-lookup"><span data-stu-id="270da-137">url</span></span>|<span data-ttu-id="270da-138">String</span><span class="sxs-lookup"><span data-stu-id="270da-138">String</span></span>|<span data-ttu-id="270da-139">TEM パートナーの管理用コントロール パネルの URL。管理者は、このパネルで TEM サービスを構成できます。</span><span class="sxs-lookup"><span data-stu-id="270da-139">URL of the TEM partner's administrative control panel, where an administrator can configure their TEM service.</span></span>|
|<span data-ttu-id="270da-140">appAuthorized</span><span class="sxs-lookup"><span data-stu-id="270da-140">appAuthorized</span></span>|<span data-ttu-id="270da-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="270da-141">Boolean</span></span>|<span data-ttu-id="270da-142">パートナーの AAD アプリに Intune へのアクセスが承認されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="270da-142">Whether the partner's AAD app has been authorized to access Intune.</span></span>|
|<span data-ttu-id="270da-143">enabled</span><span class="sxs-lookup"><span data-stu-id="270da-143">enabled</span></span>|<span data-ttu-id="270da-144">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="270da-144">Boolean</span></span>|<span data-ttu-id="270da-145">TEM サービスへの Intune の接続が現在有効であるか、無効であるかを示します。</span><span class="sxs-lookup"><span data-stu-id="270da-145">Whether Intune's connection to the TEM service is currently enabled or disabled.</span></span>|
|<span data-ttu-id="270da-146">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="270da-146">lastConnectionDateTime</span></span>|<span data-ttu-id="270da-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="270da-147">DateTimeOffset</span></span>|<span data-ttu-id="270da-148">TEM パートナーによって Intune に最後に送信された要求のタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="270da-148">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="270da-149">応答</span><span class="sxs-lookup"><span data-stu-id="270da-149">Response</span></span>
<span data-ttu-id="270da-150">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="270da-150">If successful, this method returns a `200 OK` response code and an updated [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="270da-151">例</span><span class="sxs-lookup"><span data-stu-id="270da-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="270da-152">要求</span><span class="sxs-lookup"><span data-stu-id="270da-152">Request</span></span>
<span data-ttu-id="270da-153">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="270da-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
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

### <a name="response"></a><span data-ttu-id="270da-154">応答</span><span class="sxs-lookup"><span data-stu-id="270da-154">Response</span></span>
<span data-ttu-id="270da-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="270da-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



