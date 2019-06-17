---
title: telecomExpenseManagementPartner の作成
description: 新しい telecomExpenseManagementPartner オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bd9fec5241cf10f177f77e26f73eb7a427441522
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34990352"
---
# <a name="create-telecomexpensemanagementpartner"></a><span data-ttu-id="63686-103">telecomExpenseManagementPartner の作成</span><span class="sxs-lookup"><span data-stu-id="63686-103">Create telecomExpenseManagementPartner</span></span>

> <span data-ttu-id="63686-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="63686-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="63686-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="63686-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63686-106">新しい [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="63686-106">Create a new [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="63686-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="63686-107">Prerequisites</span></span>
<span data-ttu-id="63686-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="63686-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63686-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="63686-110">Permission type</span></span>|<span data-ttu-id="63686-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="63686-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="63686-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="63686-112">Delegated (work or school account)</span></span>|<span data-ttu-id="63686-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63686-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="63686-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="63686-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="63686-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="63686-115">Not supported.</span></span>|
|<span data-ttu-id="63686-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="63686-116">Application</span></span>|<span data-ttu-id="63686-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="63686-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="63686-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="63686-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/telecomExpenseManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="63686-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="63686-119">Request headers</span></span>
|<span data-ttu-id="63686-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="63686-120">Header</span></span>|<span data-ttu-id="63686-121">値</span><span class="sxs-lookup"><span data-stu-id="63686-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="63686-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="63686-122">Authorization</span></span>|<span data-ttu-id="63686-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="63686-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="63686-124">承諾</span><span class="sxs-lookup"><span data-stu-id="63686-124">Accept</span></span>|<span data-ttu-id="63686-125">application/json</span><span class="sxs-lookup"><span data-stu-id="63686-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="63686-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="63686-126">Request body</span></span>
<span data-ttu-id="63686-127">要求本文で、telecomExpenseManagementPartner オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="63686-127">In the request body, supply a JSON representation for the telecomExpenseManagementPartner object.</span></span>

<span data-ttu-id="63686-128">次の表に、telecomExpenseManagementPartner の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="63686-128">The following table shows the properties that are required when you create the telecomExpenseManagementPartner.</span></span>

|<span data-ttu-id="63686-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="63686-129">Property</span></span>|<span data-ttu-id="63686-130">型</span><span class="sxs-lookup"><span data-stu-id="63686-130">Type</span></span>|<span data-ttu-id="63686-131">説明</span><span class="sxs-lookup"><span data-stu-id="63686-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63686-132">id</span><span class="sxs-lookup"><span data-stu-id="63686-132">id</span></span>|<span data-ttu-id="63686-133">文字列</span><span class="sxs-lookup"><span data-stu-id="63686-133">String</span></span>|<span data-ttu-id="63686-134">TEM パートナーの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="63686-134">Unique identifier of the TEM partner.</span></span>|
|<span data-ttu-id="63686-135">displayName</span><span class="sxs-lookup"><span data-stu-id="63686-135">displayName</span></span>|<span data-ttu-id="63686-136">String</span><span class="sxs-lookup"><span data-stu-id="63686-136">String</span></span>|<span data-ttu-id="63686-137">TEM パートナーの表示名。</span><span class="sxs-lookup"><span data-stu-id="63686-137">Display name of the TEM partner.</span></span>|
|<span data-ttu-id="63686-138">url</span><span class="sxs-lookup"><span data-stu-id="63686-138">url</span></span>|<span data-ttu-id="63686-139">String</span><span class="sxs-lookup"><span data-stu-id="63686-139">String</span></span>|<span data-ttu-id="63686-140">TEM パートナーの管理用コントロール パネルの URL。管理者は、このパネルで TEM サービスを構成できます。</span><span class="sxs-lookup"><span data-stu-id="63686-140">URL of the TEM partner's administrative control panel, where an administrator can configure their TEM service.</span></span>|
|<span data-ttu-id="63686-141">appAuthorized</span><span class="sxs-lookup"><span data-stu-id="63686-141">appAuthorized</span></span>|<span data-ttu-id="63686-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="63686-142">Boolean</span></span>|<span data-ttu-id="63686-143">パートナーの AAD アプリに Intune へのアクセスが承認されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="63686-143">Whether the partner's AAD app has been authorized to access Intune.</span></span>|
|<span data-ttu-id="63686-144">enabled</span><span class="sxs-lookup"><span data-stu-id="63686-144">enabled</span></span>|<span data-ttu-id="63686-145">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="63686-145">Boolean</span></span>|<span data-ttu-id="63686-146">TEM サービスへの Intune の接続が現在有効であるか、無効であるかを示します。</span><span class="sxs-lookup"><span data-stu-id="63686-146">Whether Intune's connection to the TEM service is currently enabled or disabled.</span></span>|
|<span data-ttu-id="63686-147">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="63686-147">lastConnectionDateTime</span></span>|<span data-ttu-id="63686-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="63686-148">DateTimeOffset</span></span>|<span data-ttu-id="63686-149">TEM パートナーによって Intune に最後に送信された要求のタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="63686-149">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="63686-150">応答</span><span class="sxs-lookup"><span data-stu-id="63686-150">Response</span></span>
<span data-ttu-id="63686-151">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="63686-151">If successful, this method returns a `201 Created` response code and a [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63686-152">例</span><span class="sxs-lookup"><span data-stu-id="63686-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="63686-153">要求</span><span class="sxs-lookup"><span data-stu-id="63686-153">Request</span></span>
<span data-ttu-id="63686-154">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="63686-154">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/telecomExpenseManagementPartners
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

### <a name="response"></a><span data-ttu-id="63686-155">応答</span><span class="sxs-lookup"><span data-stu-id="63686-155">Response</span></span>
<span data-ttu-id="63686-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="63686-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





