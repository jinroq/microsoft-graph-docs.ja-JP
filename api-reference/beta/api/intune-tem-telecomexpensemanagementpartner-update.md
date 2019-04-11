---
title: telecomExpenseManagementPartner の更新
description: telecomExpenseManagementPartner オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eabd6e795558ee719ef3e6c1ac79039b3ef040b7
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31794667"
---
# <a name="update-telecomexpensemanagementpartner"></a><span data-ttu-id="06435-103">telecomExpenseManagementPartner の更新</span><span class="sxs-lookup"><span data-stu-id="06435-103">Update telecomExpenseManagementPartner</span></span>

> <span data-ttu-id="06435-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="06435-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="06435-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="06435-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06435-106">[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="06435-106">Update the properties of a [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="06435-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="06435-107">Prerequisites</span></span>
<span data-ttu-id="06435-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="06435-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06435-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="06435-110">Permission type</span></span>|<span data-ttu-id="06435-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="06435-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06435-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="06435-112">Delegated (work or school account)</span></span>|<span data-ttu-id="06435-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06435-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="06435-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="06435-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06435-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="06435-115">Not supported.</span></span>|
|<span data-ttu-id="06435-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="06435-116">Application</span></span>|<span data-ttu-id="06435-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="06435-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="06435-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="06435-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="06435-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="06435-119">Request headers</span></span>
|<span data-ttu-id="06435-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="06435-120">Header</span></span>|<span data-ttu-id="06435-121">値</span><span class="sxs-lookup"><span data-stu-id="06435-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06435-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="06435-122">Authorization</span></span>|<span data-ttu-id="06435-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="06435-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06435-124">承諾</span><span class="sxs-lookup"><span data-stu-id="06435-124">Accept</span></span>|<span data-ttu-id="06435-125">application/json</span><span class="sxs-lookup"><span data-stu-id="06435-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06435-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="06435-126">Request body</span></span>
<span data-ttu-id="06435-127">要求本文で、[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="06435-127">In the request body, supply a JSON representation for the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>

<span data-ttu-id="06435-128">次の表に、[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="06435-128">The following table shows the properties that are required when you create the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span></span>

|<span data-ttu-id="06435-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="06435-129">Property</span></span>|<span data-ttu-id="06435-130">型</span><span class="sxs-lookup"><span data-stu-id="06435-130">Type</span></span>|<span data-ttu-id="06435-131">説明</span><span class="sxs-lookup"><span data-stu-id="06435-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06435-132">id</span><span class="sxs-lookup"><span data-stu-id="06435-132">id</span></span>|<span data-ttu-id="06435-133">文字列</span><span class="sxs-lookup"><span data-stu-id="06435-133">String</span></span>|<span data-ttu-id="06435-134">TEM パートナーの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="06435-134">Unique identifier of the TEM partner.</span></span>|
|<span data-ttu-id="06435-135">displayName</span><span class="sxs-lookup"><span data-stu-id="06435-135">displayName</span></span>|<span data-ttu-id="06435-136">String</span><span class="sxs-lookup"><span data-stu-id="06435-136">String</span></span>|<span data-ttu-id="06435-137">TEM パートナーの表示名。</span><span class="sxs-lookup"><span data-stu-id="06435-137">Display name of the TEM partner.</span></span>|
|<span data-ttu-id="06435-138">url</span><span class="sxs-lookup"><span data-stu-id="06435-138">url</span></span>|<span data-ttu-id="06435-139">String</span><span class="sxs-lookup"><span data-stu-id="06435-139">String</span></span>|<span data-ttu-id="06435-140">TEM パートナーの管理用コントロール パネルの URL。管理者は、このパネルで TEM サービスを構成できます。</span><span class="sxs-lookup"><span data-stu-id="06435-140">URL of the TEM partner's administrative control panel, where an administrator can configure their TEM service.</span></span>|
|<span data-ttu-id="06435-141">appAuthorized</span><span class="sxs-lookup"><span data-stu-id="06435-141">appAuthorized</span></span>|<span data-ttu-id="06435-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="06435-142">Boolean</span></span>|<span data-ttu-id="06435-143">パートナーの AAD アプリに Intune へのアクセスが承認されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="06435-143">Whether the partner's AAD app has been authorized to access Intune.</span></span>|
|<span data-ttu-id="06435-144">enabled</span><span class="sxs-lookup"><span data-stu-id="06435-144">enabled</span></span>|<span data-ttu-id="06435-145">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="06435-145">Boolean</span></span>|<span data-ttu-id="06435-146">TEM サービスへの Intune の接続が現在有効であるか、無効であるかを示します。</span><span class="sxs-lookup"><span data-stu-id="06435-146">Whether Intune's connection to the TEM service is currently enabled or disabled.</span></span>|
|<span data-ttu-id="06435-147">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="06435-147">lastConnectionDateTime</span></span>|<span data-ttu-id="06435-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06435-148">DateTimeOffset</span></span>|<span data-ttu-id="06435-149">TEM パートナーによって Intune に最後に送信された要求のタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="06435-149">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="06435-150">応答</span><span class="sxs-lookup"><span data-stu-id="06435-150">Response</span></span>
<span data-ttu-id="06435-151">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="06435-151">If successful, this method returns a `200 OK` response code and an updated [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06435-152">例</span><span class="sxs-lookup"><span data-stu-id="06435-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="06435-153">要求</span><span class="sxs-lookup"><span data-stu-id="06435-153">Request</span></span>
<span data-ttu-id="06435-154">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="06435-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
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

### <a name="response"></a><span data-ttu-id="06435-155">応答</span><span class="sxs-lookup"><span data-stu-id="06435-155">Response</span></span>
<span data-ttu-id="06435-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="06435-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





