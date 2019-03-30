---
title: windowsDefenderAdvancedThreatProtectionConfiguration の削除
description: windowsDefenderAdvancedThreatProtectionConfiguration を削除します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 42b11ef625c2e31fb29d2d612f786c258d529d53
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30988400"
---
# <a name="delete-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="c0db3-103">windowsDefenderAdvancedThreatProtectionConfiguration の削除</span><span class="sxs-lookup"><span data-stu-id="c0db3-103">Delete windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

> <span data-ttu-id="c0db3-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c0db3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0db3-105">[windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="c0db3-105">Deletes a [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c0db3-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="c0db3-106">Prerequisites</span></span>
<span data-ttu-id="c0db3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c0db3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0db3-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c0db3-109">Permission type</span></span>|<span data-ttu-id="c0db3-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c0db3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0db3-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c0db3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c0db3-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0db3-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c0db3-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c0db3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0db3-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c0db3-114">Not supported.</span></span>|
|<span data-ttu-id="c0db3-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c0db3-115">Application</span></span>|<span data-ttu-id="c0db3-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c0db3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0db3-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c0db3-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="c0db3-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c0db3-118">Request headers</span></span>
|<span data-ttu-id="c0db3-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c0db3-119">Header</span></span>|<span data-ttu-id="c0db3-120">値</span><span class="sxs-lookup"><span data-stu-id="c0db3-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c0db3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0db3-121">Authorization</span></span>|<span data-ttu-id="c0db3-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="c0db3-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c0db3-123">承諾</span><span class="sxs-lookup"><span data-stu-id="c0db3-123">Accept</span></span>|<span data-ttu-id="c0db3-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c0db3-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0db3-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="c0db3-125">Request body</span></span>
<span data-ttu-id="c0db3-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c0db3-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0db3-127">応答</span><span class="sxs-lookup"><span data-stu-id="c0db3-127">Response</span></span>
<span data-ttu-id="c0db3-128">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="c0db3-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c0db3-129">例</span><span class="sxs-lookup"><span data-stu-id="c0db3-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="c0db3-130">要求</span><span class="sxs-lookup"><span data-stu-id="c0db3-130">Request</span></span>
<span data-ttu-id="c0db3-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c0db3-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="c0db3-132">応答</span><span class="sxs-lookup"><span data-stu-id="c0db3-132">Response</span></span>
<span data-ttu-id="c0db3-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c0db3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



