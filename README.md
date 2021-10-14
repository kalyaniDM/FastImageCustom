# FastImageCustom
Added a placeholder in ios 

    UIImage *placeholderImage;
    if(_source.cacheControl==FFFCacheControlCacheOnly){
        placeholderImage=[UIImage imageNamed:@"defaultArticleImage"];
    }
    else{
        placeholderImage=nil;
    }
    __weak typeof(self) weakSelf = self; // Always use a weak reference to self in blocks
    [self sd_setImageWithURL:_source.url
            placeholderImage:placeholderImage
            
            
Steps: 
1.in FastImageView.m added code for placeholder if no image downloaded or not in cache
2.Add a placeholder image named "defaultArticleImage.png" in 1x and 2x size in ImageAssests from xcode where splash and icons are added
