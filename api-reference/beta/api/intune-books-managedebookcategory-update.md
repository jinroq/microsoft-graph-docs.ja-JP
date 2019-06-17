---
title: ManagedEBookCategory の更新
description: ManagedEBookCategory オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a4a9f9ea4d7f8c53c5dc35aed552edb6d7bbea11
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34972145"
---
# <a name="update-managedebookcategory"></a><span data-ttu-id="19953-103">ManagedEBookCategory の更新</span><span class="sxs-lookup"><span data-stu-id="19953-103">Update managedEBookCategory</span></span>

> <span data-ttu-id="19953-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="19953-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="19953-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="19953-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19953-106">[Managedebookcategory](../resources/intune-books-managedebookcategory.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="19953-106">Update the properties of a [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="19953-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="19953-107">Prerequisites</span></span>
<span data-ttu-id="19953-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="19953-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19953-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="19953-110">Permission type</span></span>|<span data-ttu-id="19953-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="19953-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="19953-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="19953-112">Delegated (work or school account)</span></span>|<span data-ttu-id="19953-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19953-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="19953-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="19953-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="19953-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="19953-115">Not supported.</span></span>|
|<span data-ttu-id="19953-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="19953-116">Application</span></span>|<span data-ttu-id="19953-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="19953-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="19953-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="19953-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBookCategories/{managedEBookCategoryId}
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/categories/{managedEBookCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="19953-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="19953-119">Request headers</span></span>
|<span data-ttu-id="19953-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="19953-120">Header</span></span>|<span data-ttu-id="19953-121">値</span><span class="sxs-lookup"><span data-stu-id="19953-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="19953-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="19953-122">Authorization</span></span>|<span data-ttu-id="19953-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="19953-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="19953-124">承諾</span><span class="sxs-lookup"><span data-stu-id="19953-124">Accept</span></span>|<span data-ttu-id="19953-125">application/json</span><span class="sxs-lookup"><span data-stu-id="19953-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="19953-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="19953-126">Request body</span></span>
<span data-ttu-id="19953-127">要求本文で、 [Managedebookcategory](../resources/intune-books-managedebookcategory.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="19953-127">In the request body, supply a JSON representation for the [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>

<span data-ttu-id="19953-128">次の表に、 [Managedebookcategory](../resources/intune-books-managedebookcategory.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="19953-128">The following table shows the properties that are required when you create the [managedEBookCategory](../resources/intune-books-managedebookcategory.md).</span></span>

|<span data-ttu-id="19953-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="19953-129">Property</span></span>|<span data-ttu-id="19953-130">型</span><span class="sxs-lookup"><span data-stu-id="19953-130">Type</span></span>|<span data-ttu-id="19953-131">説明</span><span class="sxs-lookup"><span data-stu-id="19953-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19953-132">id</span><span class="sxs-lookup"><span data-stu-id="19953-132">id</span></span>|<span data-ttu-id="19953-133">文字列</span><span class="sxs-lookup"><span data-stu-id="19953-133">String</span></span>|<span data-ttu-id="19953-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="19953-134">The key of the entity.</span></span>|
|<span data-ttu-id="19953-135">displayName</span><span class="sxs-lookup"><span data-stu-id="19953-135">displayName</span></span>|<span data-ttu-id="19953-136">String</span><span class="sxs-lookup"><span data-stu-id="19953-136">String</span></span>|<span data-ttu-id="19953-137">EBook カテゴリの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="19953-137">The name of the eBook category.</span></span>|
|<span data-ttu-id="19953-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="19953-138">lastModifiedDateTime</span></span>|<span data-ttu-id="19953-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19953-139">DateTimeOffset</span></span>|<span data-ttu-id="19953-140">ManagedEBookCategory が最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="19953-140">The date and time the ManagedEBookCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="19953-141">応答</span><span class="sxs-lookup"><span data-stu-id="19953-141">Response</span></span>
<span data-ttu-id="19953-142">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[Managedebookcategory](../resources/intune-books-managedebookcategory.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="19953-142">If successful, this method returns a `200 OK` response code and an updated [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19953-143">例</span><span class="sxs-lookup"><span data-stu-id="19953-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="19953-144">要求</span><span class="sxs-lookup"><span data-stu-id="19953-144">Request</span></span>
<span data-ttu-id="19953-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="19953-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBookCategories/{managedEBookCategoryId}
Content-type: application/json
Content-length: 102

{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="19953-146">応答</span><span class="sxs-lookup"><span data-stu-id="19953-146">Response</span></span>
<span data-ttu-id="19953-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="19953-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 215

{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "id": "3c71fb14-fb14-3c71-14fb-713c14fb713c",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```





