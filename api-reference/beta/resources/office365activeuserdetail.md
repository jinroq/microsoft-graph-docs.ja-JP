---
title: office365ActiveUserDetail リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 9e58e0d4613118cd8ceecfcae318982bc2035917
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009497"
---
# <a name="office365activeuserdetail-resource-type"></a><span data-ttu-id="74d99-103">office365ActiveUserDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="74d99-103">office365ActiveUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="74d99-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="74d99-104">Properties</span></span>

| <span data-ttu-id="74d99-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="74d99-105">Property</span></span>                          | <span data-ttu-id="74d99-106">型</span><span class="sxs-lookup"><span data-stu-id="74d99-106">Type</span></span>              | <span data-ttu-id="74d99-107">説明</span><span class="sxs-lookup"><span data-stu-id="74d99-107">Description</span></span>                              |
| :-------------------------------- | :---------------- | ---------------------------------------- |
| <span data-ttu-id="74d99-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="74d99-108">reportRefreshDate</span></span>                 | <span data-ttu-id="74d99-109">日付</span><span class="sxs-lookup"><span data-stu-id="74d99-109">Date</span></span>              | <span data-ttu-id="74d99-110">コンテンツの最新の日付。</span><span class="sxs-lookup"><span data-stu-id="74d99-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="74d99-111">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="74d99-111">userPrincipalName</span></span>                 | <span data-ttu-id="74d99-112">String</span><span class="sxs-lookup"><span data-stu-id="74d99-112">String</span></span>            | <span data-ttu-id="74d99-113">ユーザーのユーザープリンシパル名 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="74d99-113">The user principal name (UPN) of the user.</span></span> <span data-ttu-id="74d99-114">UPN は、インターネット標準 RFC 822 に基づくユーザーのインターネットスタイルのログイン名です。</span><span class="sxs-lookup"><span data-stu-id="74d99-114">The UPN is an Internet-style login name for the user based on the Internet standard RFC 822.</span></span> <span data-ttu-id="74d99-115">規則により、これはユーザーの電子メール名にマップする必要があります。</span><span class="sxs-lookup"><span data-stu-id="74d99-115">By convention, this should map to the user's email name.</span></span> <span data-ttu-id="74d99-116">一般的な形式は、検証済みドメインのテナントのコレクションにドメインが存在する必要がある、エイリアス @ domain です。</span><span class="sxs-lookup"><span data-stu-id="74d99-116">The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains.</span></span> <span data-ttu-id="74d99-117">このプロパティは、ユーザーの作成時に必要です。</span><span class="sxs-lookup"><span data-stu-id="74d99-117">This property is required when a user is created.</span></span> |
| <span data-ttu-id="74d99-118">displayName</span><span class="sxs-lookup"><span data-stu-id="74d99-118">displayName</span></span>                       | <span data-ttu-id="74d99-119">文字列</span><span class="sxs-lookup"><span data-stu-id="74d99-119">String</span></span>            | <span data-ttu-id="74d99-120">アドレス帳に表示されるユーザーの名前。</span><span class="sxs-lookup"><span data-stu-id="74d99-120">The name displayed in the address book for the user.</span></span> <span data-ttu-id="74d99-121">これは通常、ユーザーの名前、ミドルネームのイニシャル、姓の組み合わせになります。</span><span class="sxs-lookup"><span data-stu-id="74d99-121">This is usually the combination of the user's first name, middle initial, and last name.</span></span> <span data-ttu-id="74d99-122">このプロパティはユーザーの作成時に必須です。更新時にクリアすることはできません。</span><span class="sxs-lookup"><span data-stu-id="74d99-122">This property is required when a user is created and it cannot be cleared during updates.</span></span> |
| <span data-ttu-id="74d99-123">isDeleted</span><span class="sxs-lookup"><span data-stu-id="74d99-123">isDeleted</span></span>                         | <span data-ttu-id="74d99-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="74d99-124">Boolean</span></span>           | <span data-ttu-id="74d99-125">このユーザーが削除されているか、または削除されているか。</span><span class="sxs-lookup"><span data-stu-id="74d99-125">Whether this user has been deleted or soft deleted.</span></span> |
| <span data-ttu-id="74d99-126">deletedDate</span><span class="sxs-lookup"><span data-stu-id="74d99-126">deletedDate</span></span>                       | <span data-ttu-id="74d99-127">日付</span><span class="sxs-lookup"><span data-stu-id="74d99-127">Date</span></span>              | <span data-ttu-id="74d99-128">削除操作が発生した日付。</span><span class="sxs-lookup"><span data-stu-id="74d99-128">The date when the delete operation happened.</span></span> <span data-ttu-id="74d99-129">ユーザーが削除されていない場合、既定値は "null" です。</span><span class="sxs-lookup"><span data-stu-id="74d99-129">Default value is "null" when the user has not been deleted.</span></span> |
| <span data-ttu-id="74d99-130">hasExchangeLicense</span><span class="sxs-lookup"><span data-stu-id="74d99-130">hasExchangeLicense</span></span>                | <span data-ttu-id="74d99-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="74d99-131">Boolean</span></span>           | <span data-ttu-id="74d99-132">ユーザーに Exchange ライセンスが割り当てられているかどうか。</span><span class="sxs-lookup"><span data-stu-id="74d99-132">Whether the user has been assigned an Exchange license.</span></span> |
| <span data-ttu-id="74d99-133">hasOneDriveLicense</span><span class="sxs-lookup"><span data-stu-id="74d99-133">hasOneDriveLicense</span></span>                | <span data-ttu-id="74d99-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="74d99-134">Boolean</span></span>           | <span data-ttu-id="74d99-135">ユーザーに OneDrive ライセンスが割り当てられているかどうか。</span><span class="sxs-lookup"><span data-stu-id="74d99-135">Whether the user has been assigned a OneDrive license.</span></span> |
| <span data-ttu-id="74d99-136">hasSharePointLicense</span><span class="sxs-lookup"><span data-stu-id="74d99-136">hasSharePointLicense</span></span>              | <span data-ttu-id="74d99-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="74d99-137">Boolean</span></span>           | <span data-ttu-id="74d99-138">ユーザーに SharePoint ライセンスが割り当てられているかどうか。</span><span class="sxs-lookup"><span data-stu-id="74d99-138">Whether the user has been assigned a SharePoint license.</span></span> |
| <span data-ttu-id="74d99-139">hasSkypeForBusinessLicense</span><span class="sxs-lookup"><span data-stu-id="74d99-139">hasSkypeForBusinessLicense</span></span>        | <span data-ttu-id="74d99-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="74d99-140">Boolean</span></span>           | <span data-ttu-id="74d99-141">ユーザーに Skype For Business ライセンスが割り当てられているかどうか。</span><span class="sxs-lookup"><span data-stu-id="74d99-141">Whether the user has been assigned a Skype For Business license.</span></span> |
| <span data-ttu-id="74d99-142">hasYammerLicense</span><span class="sxs-lookup"><span data-stu-id="74d99-142">hasYammerLicense</span></span>                  | <span data-ttu-id="74d99-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="74d99-143">Boolean</span></span>           | <span data-ttu-id="74d99-144">ユーザーに Yammer ライセンスが割り当てられているかどうか。</span><span class="sxs-lookup"><span data-stu-id="74d99-144">Whether the user has been assigned a Yammer license.</span></span> |
| <span data-ttu-id="74d99-145">hasTeamsLicense</span><span class="sxs-lookup"><span data-stu-id="74d99-145">hasTeamsLicense</span></span>                   | <span data-ttu-id="74d99-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="74d99-146">Boolean</span></span>           | <span data-ttu-id="74d99-147">ユーザーに Teams ライセンスが割り当てられているかどうか。</span><span class="sxs-lookup"><span data-stu-id="74d99-147">Whether the user has been assigned a Teams license.</span></span> |
| <span data-ttu-id="74d99-148">exchangeLastActivityDate</span><span class="sxs-lookup"><span data-stu-id="74d99-148">exchangeLastActivityDate</span></span>          | <span data-ttu-id="74d99-149">日付</span><span class="sxs-lookup"><span data-stu-id="74d99-149">Date</span></span>              | <span data-ttu-id="74d99-150">ユーザーが最後に電子メールを読んだり送信したりした日付。</span><span class="sxs-lookup"><span data-stu-id="74d99-150">The date when user last read or sent email.</span></span> |
| <span data-ttu-id="74d99-151">oneDriveLastActivityDate</span><span class="sxs-lookup"><span data-stu-id="74d99-151">oneDriveLastActivityDate</span></span>          | <span data-ttu-id="74d99-152">日付</span><span class="sxs-lookup"><span data-stu-id="74d99-152">Date</span></span>              | <span data-ttu-id="74d99-153">ユーザーが最後にファイルを表示または編集した日付、共有ファイルの内部または外部、または同期したファイル。</span><span class="sxs-lookup"><span data-stu-id="74d99-153">The date when user last viewed or edited files, shared files internally or externally, or synced files.</span></span> |
| <span data-ttu-id="74d99-154">sharePointLastActivityDate</span><span class="sxs-lookup"><span data-stu-id="74d99-154">sharePointLastActivityDate</span></span>        | <span data-ttu-id="74d99-155">日付</span><span class="sxs-lookup"><span data-stu-id="74d99-155">Date</span></span>              | <span data-ttu-id="74d99-156">ユーザーが最後にファイルを表示または編集した日付、共有ファイルの内部または外部、同期済みファイル、または SharePoint ページを表示した日付。</span><span class="sxs-lookup"><span data-stu-id="74d99-156">The date when user last viewed or edited files, shared files internally or externally, synced files, or viewed SharePoint pages.</span></span> |
| <span data-ttu-id="74d99-157">skypeForBusinessLastActivityDate</span><span class="sxs-lookup"><span data-stu-id="74d99-157">skypeForBusinessLastActivityDate</span></span>  | <span data-ttu-id="74d99-158">日付</span><span class="sxs-lookup"><span data-stu-id="74d99-158">Date</span></span>              | <span data-ttu-id="74d99-159">ユーザーが会議に最後に開催または参加した日付、またはピアツーピアセッションに参加した日付。</span><span class="sxs-lookup"><span data-stu-id="74d99-159">The date when user last organized or participated in conferences, or joined peer-to-peer sessions.</span></span> |
| <span data-ttu-id="74d99-160">yammerLastActivityDate</span><span class="sxs-lookup"><span data-stu-id="74d99-160">yammerLastActivityDate</span></span>            | <span data-ttu-id="74d99-161">日付</span><span class="sxs-lookup"><span data-stu-id="74d99-161">Date</span></span>              | <span data-ttu-id="74d99-162">ユーザーが最後に投稿、閲覧、または「いいね!」のメッセージを最後に投稿した日付。</span><span class="sxs-lookup"><span data-stu-id="74d99-162">The date when user last posted, read, or liked message.</span></span> |
| <span data-ttu-id="74d99-163">teamsLastActivityDate</span><span class="sxs-lookup"><span data-stu-id="74d99-163">teamsLastActivityDate</span></span>             | <span data-ttu-id="74d99-164">日付</span><span class="sxs-lookup"><span data-stu-id="74d99-164">Date</span></span>              | <span data-ttu-id="74d99-165">ユーザーがチームチャネルでメッセージを最後に投稿した日、プライベートチャットセッションでメッセージを送信した、または会議または通話に参加した日付。</span><span class="sxs-lookup"><span data-stu-id="74d99-165">The date when user last posted messages in team channels, sent messages in private chat sessions, or participated in meetings or calls.</span></span> |
| <span data-ttu-id="74d99-166">exchangeLicenseAssignDate</span><span class="sxs-lookup"><span data-stu-id="74d99-166">exchangeLicenseAssignDate</span></span>         | <span data-ttu-id="74d99-167">日付</span><span class="sxs-lookup"><span data-stu-id="74d99-167">Date</span></span>              | <span data-ttu-id="74d99-168">ユーザーが Exchange ライセンスを割り当てられた最後の日付。</span><span class="sxs-lookup"><span data-stu-id="74d99-168">The last date when the user was assigned an Exchange license.</span></span> |
| <span data-ttu-id="74d99-169">oneDriveLicenseAssignDate</span><span class="sxs-lookup"><span data-stu-id="74d99-169">oneDriveLicenseAssignDate</span></span>         | <span data-ttu-id="74d99-170">日付</span><span class="sxs-lookup"><span data-stu-id="74d99-170">Date</span></span>              | <span data-ttu-id="74d99-171">ユーザーが OneDrive ライセンスを割り当てられた最後の日付。</span><span class="sxs-lookup"><span data-stu-id="74d99-171">The last date when the user was assigned a OneDrive license.</span></span> |
| <span data-ttu-id="74d99-172">Sharepointlicenseの割り当て日付</span><span class="sxs-lookup"><span data-stu-id="74d99-172">sharePointLicenseAssignDate</span></span>       | <span data-ttu-id="74d99-173">日付</span><span class="sxs-lookup"><span data-stu-id="74d99-173">Date</span></span>              | <span data-ttu-id="74d99-174">ユーザーが SharePoint ライセンスを割り当てられた最後の日付。</span><span class="sxs-lookup"><span data-stu-id="74d99-174">The last date when the user was assigned a SharePoint license.</span></span> |
| <span data-ttu-id="74d99-175">Skypeforbusinesslicenseの割り当て日付</span><span class="sxs-lookup"><span data-stu-id="74d99-175">skypeForBusinessLicenseAssignDate</span></span> | <span data-ttu-id="74d99-176">日付</span><span class="sxs-lookup"><span data-stu-id="74d99-176">Date</span></span>              | <span data-ttu-id="74d99-177">ユーザーが Skype For Business ライセンスを割り当てられた最後の日付。</span><span class="sxs-lookup"><span data-stu-id="74d99-177">The last date when the user was assigned a Skype For Business license.</span></span> |
| <span data-ttu-id="74d99-178">yammerLicenseAssignDate</span><span class="sxs-lookup"><span data-stu-id="74d99-178">yammerLicenseAssignDate</span></span>           | <span data-ttu-id="74d99-179">日付</span><span class="sxs-lookup"><span data-stu-id="74d99-179">Date</span></span>              | <span data-ttu-id="74d99-180">ユーザーが Yammer ライセンスを割り当てられた最後の日付。</span><span class="sxs-lookup"><span data-stu-id="74d99-180">The last date when the user was assigned a Yammer license.</span></span> |
| <span data-ttu-id="74d99-181">Teamslicenseの割り当て日付</span><span class="sxs-lookup"><span data-stu-id="74d99-181">teamsLicenseAssignDate</span></span>            | <span data-ttu-id="74d99-182">日付</span><span class="sxs-lookup"><span data-stu-id="74d99-182">Date</span></span>              | <span data-ttu-id="74d99-183">ユーザーが Teams ライセンスを割り当てられた最後の日付。</span><span class="sxs-lookup"><span data-stu-id="74d99-183">The last date when the user was assigned a Teams license.</span></span> |
| <span data-ttu-id="74d99-184">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="74d99-184">assignedProducts</span></span>                  | <span data-ttu-id="74d99-185">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="74d99-185">String collection</span></span> | <span data-ttu-id="74d99-186">ユーザーに割り当てられているすべての製品。</span><span class="sxs-lookup"><span data-stu-id="74d99-186">All the products assigned for the user.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="74d99-187">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="74d99-187">JSON representation</span></span>

<span data-ttu-id="74d99-188">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="74d99-188">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ActiveUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "hasExchangeLicense": true, 
  "hasOneDriveLicense": true, 
  "hasSharePointLicense": true, 
  "hasSkypeForBusinessLicense": true, 
  "hasYammerLicense": true, 
  "hasTeamsLicense": true, 
  "exchangeLastActivityDate": "Date", 
  "oneDriveLastActivityDate": "Date", 
  "sharePointLastActivityDate": "Date", 
  "skypeForBusinessLastActivityDate": "Date", 
  "yammerLastActivityDate": "Date", 
  "teamsLastActivityDate": "Date", 
  "exchangeLicenseAssignDate": "Date", 
  "oneDriveLicenseAssignDate": "Date", 
  "sharePointLicenseAssignDate": "Date", 
  "skypeForBusinessLicenseAssignDate": "Date", 
  "yammerLicenseAssignDate": "Date", 
  "teamsLicenseAssignDate": "Date", 
  "assignedProducts": ["String"]
}
```
